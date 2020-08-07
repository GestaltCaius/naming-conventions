SQL Tables and Columns naming conventions
===

* Table and column names should use Pascal casing (upper camel case e.g. PostalCode)
* Table names could either be singular or plural. It comes down to personal preference
* Singular names for columns
* Table’s ID must be prefixed by table’s name in its singular form (e.g. CustomerID, even though your table is named Customers)
* Foreign key names must be consistent
* Do not use abbreviations in your column names. It makes things harder to understand.

> Back in the days, table et column names were using ALLCAPS and underscores names.
> According to this stackoverflow thread, it’s not the convention anymore.

Example:

```sql
Table Customer(s)

int CustomerID (PK)
varchar Email
varchar PasswordHash -- PasswordPBKDF2Hash might be a better name to make things clearer?
int OrderID (FK)
```

# References

* (https://stackoverflow.com/questions/7662/database-table-and-column-naming-conventions)[Database, Table and Column Naming Conventions? [closed]]
  * (https://stackoverflow.com/questions/7662/database-table-and-column-naming-conventions/7724#7724)[Réponse 1]
  * (https://stackoverflow.com/questions/7662/database-table-and-column-naming-conventions/2118567#2118567)[Réponse 2 (plus détaillée, avec des explications; etc.)]
