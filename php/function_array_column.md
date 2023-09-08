# array_column()

extracts the elements from an array (or an object), by their name

Code example:

```php
$hashmapCollection = [
    ["firstname"=>"Leonid", "lastname"=>"Brezhnev"],
    ["firstname"=>"Yuri", "lastname"=>"Andropov"],
    ["firstname"=>"Konstantin", "lastname"=>"Chernenko"]
    ];
    
    
    print_r(array_column($hashmapCollection, 'lastname'));

Output:
Array
(
    [0] => Brezhnev
    [1] => Andropov
    [2] => Chernenko
)
```


https://3v4l.org/lSOg2

The third argument is used when building the returned array, to create a hash.

```php
$hashmapCollection = [
    ["firstname"=>"Leonid", "lastname"=>"Brezhnev"],
    ["firstname"=>"Yuri", "lastname"=>"Andropov"],
    ["firstname"=>"Konstantin", "lastname"=>"Chernenko"]
    ];
    
    
    print_r(array_column($hashmapCollection, 'lastname', 'firstname'));

Output:
Array
(
    [Leonid] => Brezhnev
    [Yuri] => Andropov
    [Konstantin] => Chernenko
)
```

https://3v4l.org/c4Z0G


source: https://www.exakat.io/en/14-php-arguments-that-are-not-enough-used/