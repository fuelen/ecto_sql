Ecto SQL
=========
[![Build Status](https://travis-ci.org/elixir-ecto/ecto_sql.svg?branch=master)](https://travis-ci.org/elixir-ecto/ecto_sql)

Ecto SQL ([documentation](https://hexdocs.pm/ecto_sql)) provides building blocks for writing SQL adapters for Ecto. It features:

  * The Ecto.Adapters.SQL module as an entry point for all SQL-based adapters
  * Default implementations for Postgres (Ecto.Adapters.Postgres) and MySQL (Ecto.Adapters.MySQL)
  * A test sandbox (Ecto.Adapters.SQL.Sandbox) that concurrently run database tests inside transactions
  * Support for database migrations via Mix tasks

To learn more about getting started, [see the Ecto repository](https://github.com/elixir-ecto/ecto). 

## Running tests

Clone the repo and fetch its dependencies:

    $ git clone https://github.com/elixir-ecto/ecto_sql.git
    $ cd ecto_sql
    $ mix deps.get
    $ mix test.all

You can also use a local Ecto checkout if desired:

    $ ECTO_PATH=../ecto mix test.all

You can run tests against an specific Ecto adapter by using the `ECTO_ADAPTER` environment variable:

    $ ECTO_ADAPTER=pg mix test

## Copyright and License

"Ecto" and the Ecto logo are copyright (c) 2012 Plataformatec.

Ecto source code is licensed under the [Apache 2 License](LICENSE.md).
