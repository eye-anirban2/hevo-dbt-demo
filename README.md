# hevo-dbt-demo

Sample dbt project for a Hevo Edge Transformations demo.

- `seeds/` holds sample raw data (customers, orders, payments) that `dbt build` loads into the warehouse.
- `models/staging/` cleans the raw tables (views).
- `models/marts/` builds the `customers` and `orders` tables for reporting.
- Tests in the `_*.yml` files check keys, accepted values and relationships.

Hevo runs this project through Transformations jobs: CI on pull requests, Merge after a merge to `main`, and Deploy on demand or on a schedule.
