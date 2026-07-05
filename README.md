# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## Local setup

```sh
rbenv install 3.2.6 # if needed
rbenv local 3.2.6
bundle install
bin/rails db:prepare
bin/rails server
```

The app runs at http://127.0.0.1:3000 by default.

Database settings can be overridden with `DATABASE_USERNAME`,
`DATABASE_PASSWORD`, `DATABASE_HOST`, and `DATABASE_PORT`. The defaults target a
local MySQL server on `127.0.0.1:3306`.

If you use the `db` service from `compose.yaml` as the local database, start it
and run Rails with:

```sh
DATABASE_PASSWORD=password DATABASE_PORT=3307 bin/rails db:prepare
DATABASE_PASSWORD=password DATABASE_PORT=3307 bin/rails server
```
