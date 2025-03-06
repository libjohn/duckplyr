# README

<!-- badges: start -->

<!-- badges: end -->

Part of the [RforLunch](https://Rfun.library.duke.edu/) workshop series, this workshop focusses on the {[duckplyr} package](https://duckplyr.tidyverse.org/).

> duckplyr package will run all of your existing dplyr code with identical results, using [DuckDB](https://duckdb.org/) where possible to compute the results faster. In addition, you can analyze larger-than-memory datasets straight from files on your disk or from the web.

-   **Center for Data and Visualization Sciences**: [/data](https://library.duke.edu/data) or [AskData](mailto:askdata@duke.edu)

-   R is memory bound

-   Larger than RAM computing demands alternative compute options

    -   RDBMS

    -   Cluster computing (or parallel)

    -   Throwing RAM at the problem

    -   Refactoring code

-   Database Management

    -   Database Administration is expensive (cost or time)

        -   Must become familiar with SQL

        -   Offload processing to a more efficient, less RAM intensive operation

    -   {DBI} and {dbplyr}

        -   Focus is on querrying

        -   DBI brokers the connection to the database

        -   dbplyr translates dplyr verbs into SQL

        -   Works with MySQL, Postgres, MSSQL, SQLite, etc.

        -   Database Administration is still required

    -   DuckDB

        -   A revolution in database management

        -   Becomes a subprocess of the parent (R will be the parent)

        -   Column-oriented (tall) rather than row-oriented

        -   More efficient for querrying

            -   Similar to how Parquet files are more efficient than CSV

                -   Parquet files also preserve schema (data typing) and use compression

    -   Demo

        -   01_basic

        -   02_ingest

    -   Hands on with Taxi data

        -   02_taxi_data

    -   See More R learning resources at [Rfun.library.duke.edu](https://rfun.library.duke.edu)
