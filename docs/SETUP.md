# Tableau workbook setup and handover

- **Tool:** Tableau Desktop compatible with workbook XML version 2023.1 family.
- **Data source:** External SQL Server, custom SQL selecting employee fields from `dbo.employees`.
- **Included data:** None; workbook `.twb` is XML and contains no SQL Server table data.
- **Credentials:** Never commit passwords or connection strings containing secrets.
- **Privacy:** Employee and salary records may be confidential; use anonymized, authorized data before recording screenshots.
- **Portability:** Adjust the SQL Server connection and database name using Tableau's data-source editor. The saved local host is not guaranteed to resolve elsewhere.
- **Verification needed:** connection, query result, dimensions, measures, filters and screenshot after refresh.
- **Related audit:** A byte-identical `Dashboard.twb` has been uploaded to EdTech-Analysis; do not describe it as EdTech-specific visualization without modifying and validating its data model.
