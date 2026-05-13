# SQL Courses

## Foundation

The foundation course is for beginners to SQL. It covers:

* the SELECT statement to retrieve data,
* column lists,
* the WHERE clause to filter data,
* the ORDER BY clause to sort data,
* creating calculated columns,
* the GROUP BY clause and aggregation functions such as COUNT() and SUM() to summarise data, and
* an introduction to joining tables to return a dataset that combines data from more than one table.

## Intermediate

The intermediate course follows on from the foundation course. It covers:

* more detailed examples of joining tables e.g. LEFT and OUTER joins,
* sub-queries,
* common table expressions (CTEs),
* temporary tables,
* the CASE statement, and
* dealing with NULLs (missing values).

## Advanced

The advanced course follows on from the intermediate course. It covers:

* Window functions and their uses e.g., ratio calculations, cumulative totals, finding the top N items in each category and
* creating and using tally tables

## Setup

### Keybinding: Run SQL with F5

VS Code does not support workspace-level keybindings, so this must be set up manually. To bind F5 to **Execute Current Statement**:

1. Open the Command Palette (`Ctrl+Shift+P`) and search for **Preferences: Open Keyboard Shortcuts (JSON)**.
1. Add the following entry to the array:

```json
{
    "key": "f5",
    "command": "mssql.executeCurrentStatement",
    "when": "editorLangId == sql"
}
```

1. Save the file. F5 will now execute the SQL statement at the cursor.
