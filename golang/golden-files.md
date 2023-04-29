# Golden files

Golden Files are a way to store a function or API reference response.

I first heard about them in a Go class at Otus.

```go
import (
	"flag"
	"io/ioutil"
	"path/filepath"
	"testing"
)

var update = flag.Bool("update", false, "update golden files")

func TestSomething(t *testing.T) {
	actual := doSomething()
	golden := filepath.Join("test-fixtures", "expected.golden")
	if *update {
		ioutil.WriteFile(golden, actual, 0644)
	}
	expected, _ := ioutil.ReadFile(golden)
	require.Equal(t, expected, actual)
}
```

```
go test -update=true
```

To see this approach, please visit https://medium.com/soon-london/testing-with-golden-files-in-go-7fccc71c43d3