# Goose out-of-order migrations

To be able to migrate goose with a timestamp less than the last completed migration, you should use the -allow-missing flag.

see: [goose/blog](https://pressly.github.io/goose/blog/2021/out-of-order-migrations/)