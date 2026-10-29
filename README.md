# Tableau Employee Data Dashboard | Workbook Source

A **Tableau Desktop workbook** built against a Microsoft SQL Server employee dataset. The tracked artifact is a Tableau `.twb` file, which contains workbook definitions and connection information—not embedded copies of the underlying SQL data.

> **Reproducibility status:** Source workbook is available; the referenced employee table and SQL Server environment are **not** included. Visual results and live refresh have not been verified on a clean machine.

## Files

| File | Description |
|---|---|
| [tableau/Dashboard.twb](tableau/Dashboard.twb) | Editable Tableau workbook definition |
| [docs/SETUP.md](docs/SETUP.md) | Data-source requirements, validation and migration guidance |

## Observed technical design

The workbook XML references an **external Microsoft SQL Server** connection and a custom SQL query using employee fields including `employee_id`, `department_id`, `hire_date`, `manager_id`, `name` and `salary`. It does **not** contain a published data extract in this repository.

Tableau Desktop is the correct authoring tool; SQL Server with a suitable example dataset is required to reproduce the report. Repoint the connection to a database you are authorized to use and inspect the custom query before refreshing.

## Open the dashboard

1. Download [the workbook](tableau/Dashboard.twb).
2. Open in a compatible Tableau Desktop version.
3. Edit the embedded data-source connection to point to an authorized SQL Server instance that contains compatible `dbo.employees` fields.
4. Validate relationships, refresh, calculated fields and visualization filters.
5. If sharing an extract-enabled copy, review the data for employee privacy before publishing.

The same workbook blob was also found in the EdTech project. **This workbook is employee-oriented, not an EdTech app dashboard**. Keep its identity clear in project documentation.

## Boundaries

No packaged source CSV, Tableau extract, verified screenshots or live Tableau Public link are provided. The workbook may contain a historic local SQL Server host name, so **do not treat it as a ready-to-connect public demo**. There is no claim that the underlying dataset is licensed for redistribution.

A lightweight repository check validates the XML file and its presence; it does not validate data connectivity.

Maintained by [bhagabatabrahma0106-dotcom](https://github.com/bhagabatabrahma0106-dotcom).
