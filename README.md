# dbt-trino-iceberg
## Installation
In your `packages.yml`:
```
packages:
  - git: "https://github.com/robbertDM/dbt-trino-iceberg"
    revision: 0.1.0
```

In your `dbt_project.yml`:
```
dispatch:
  - macro_namespace: dbt
    search_order: ['dbt_trino_iceberg', *project_name, 'dbt']
```
Where `*project_name` is the name of your project.

Then, run `dbt deps`. You should be good to go.
