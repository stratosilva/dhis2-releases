# 2.34 Upgrade Notes

## Tomcat support

- Minimum required Tomcat version is now **8.5.50**. Support for Tomcat 7.0 and 8.0 is now dropped. The main reason for this change is Tomcat 7.0 and 8.0 having several issues with certain application development frameworks (most importantly _Jackson_, used for JSON and XML serialization) used internally by DHIS 2. 

## Web API and Data model

- A new entity and API resource is introduced called `Visualization`, found at `/api/visualizations`. This entity merged the previous `ReportTable` and `Chart` entities and API resources. The corresponding API endpoints `/api/reportTables` and `/api/charts` will be functional for some time, but will be removed in the future and we recommend clients to migrate as soon as possible. This also implies that report tables and charts cannot be exchanged between systems using the `/api/metadata` endpint. Instead, metadata should be exchanged as visualizations.

- The `/api/configuration/settings` and `/api/configuration/settings` endpoints have been removed.

## Process
