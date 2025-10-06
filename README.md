# Dataform ITISCX Repository

### A dataform repository contains the following types of files

Config files

- These files configure your Dataform project and contain Javascript dependencies. The dataform.json, contains general information that Dataform uses to create new tables and views. Such as which schema should be used.
- In the package.json all the Javascript dependencies are found.

Definitions

- Definitions are SQLX and JavaScript files that define new tables, views, and additional SQL operations to run in BigQuery. These files are organized according to their data stage.
- An SQLX file consists of a block and body. The body contains the SQL specific information. The block specifies the output of the script. Additionally it contains documentation and data quality tests.

Includes

- It contains JavaScript files where you can define variables and functions.

### The inital dataform files are configured using the 'main' branch. However at runtime, compilation overrides makes sure that each stage contains the branch specific parameters

### Developers can create workspaces within the 'dev' repository in Dataform, allowing them to experiment with and test new features. For each developer a different schema will be used to store created tables and views, within the same dataset in BigQuery
