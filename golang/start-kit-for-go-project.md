# Start kit for go projects


To start a project in spring & java there is [spring-io/initializr](https://start.spring.io/) [Source on github](https://github.com/spring-io/initializr/)

For Golang, I found https://autostrada.dev/

It creates an zip archive, with a preset structure and interesting packages for frequent tasks.

It was useful for me to see the use of such libraries in the project:
- github.com/pascaldekloe/jwt to handle jwt authorisation
- github.com/alexedwards/flow for routing
- https://github.com/cosmtrek/air Live reload for Go apps

Unfortunately the interaction with PostgreSql is done via github.com/lib/pq instead of pgx (but this is already in the roadmap, will be fixed soon)
