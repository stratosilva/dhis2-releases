# DHIS2 version 40 Release Note

## ANALYTICS FEATURES

**On-the-fly custom calculations in Data Visualizer:** Now it's even easier to explore your data within DHIS2! With this feature, you can create your own custom calculations directly in the application for pivot tables. This means you no longer need to have admin access or create new indicators to play around with your own personal data expressions. Plus, the custom calculation is automatically saved to the pivot table in which it was created, without cluttering up your configuration with additional saved indicators. This feature is perfect for things like exploring coverage calculations with various population denominators or making quick and simple sums.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13871)

**Enhance single value charts with legend colors:** Now, legend colors can be applied to the background of a single value chart, making the performance of the value more obvious and visually engaging. This feature helps users quickly understand the significance of the value and its relation to the legend colors.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13702)

**Legend for stacked column charts:** Spice up your data visualizations with a new feature that allows legends to be applied to column charts! This makes it easier to see how indicators are performing at a glance.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13783)

**Data element and indicator icons for single value charts:** Want to add some personality to your data? Now, icons can be shown in single value charts to represent the data element or indicator being used. For example, if you're tracking total malaria cases, you can choose a mosquito icon to visually communicate what the value represents.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-5497)

**Linelists on dashboards:** Keep track of all your data in one place with line lists now available on dashboards! This feature has also been added to the latest releases of 2.39 and 2.38.  
[Jira](https://dhis2.atlassian.net/browse/TECH-475)

**Multiple event coordinate types in maps:** Visualize geographical data in new ways with multiple event coordinate types now available for use in maps. Choose to view location by event coordinate, enrollment coordinate, tracked entity coordinate, program stage data elements of type coordinates, or program tracked entity attributes of type coordinate. For example, easily see the household location for women who delivered last week at the health facility for outreach services.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-8165)

**Display values in thematic layers:** Make your maps even more informative with the option to show values directly on the map in thematic layers. This addition complements the legend and provides a more complete picture of the data being presented.  
[Jira](https://jira.dhis2.org/browse/DHIS2-13356)

**New predictor functions for computing probability:** In supply chain applications, knowing the probability of a stock out is crucial. With the new predictor functions for normDistCum and normDistDen, you can compute the probability of a stock out for normally distributed stock consumption. These functions provide the equivalent of Excel NORM.DIST() and LibreOffice NORMDIST() and allow you to calculate the probability density function (PDF) and cumulative distribution function (CDF) for a given mean and standard deviation.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14714)

**Efficiently create multiple predictors with data element groups:** Streamline your work with predictors by applying them to data element groups. This time-saving feature allows you to make multiple predictors, based on the data elements in a group, from a single definition. For instance, if you're tracking data for multiple commodities in supply chain, simply apply the predictor to the data element group for each commodity to produce the necessary values.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14635)


## TRACKER AND EVENT FEATURES

**Breaking the glass:**
The Capture app now supports programs with an access level of "protected." This means that if you're a clinician in one clinic and need to access records from another clinic, you'll be prompted to provide a reason for why you need access. This feature is especially handy for users who need to access their own records regularly but only occasionally need access to records from other organisation units. This functionality has been re-implemented in Capture in an even better form than the old Tracker Capture. To take advantage of this feature, make sure you're using DHIS version 2.38 or higher and Capture version 100.27.0 or higher.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13804)

**Saved program stage working lists for tracker programs:**
Program stage filters have been partially supported in the Capture app since 2.39, allowing filtering and ordering of lists based on event data in tracker programs. In 2.40 these filters can also be stored and shared as working lists. The program stage working lists can be utilized for many different purposes. Some examples are creating followup lists of specific tasks, following up defaulters or systematically reviewing data.
Supported in DHIS2 version 40 or higher, with capture version 100.X.0 or higher.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13654)

**Headerbar improvements:**
The header bar in Capture app has been updated to match other apps in the system. While the functionality remains the same, the header now takes up less space, and popovers are used to avoid situations where the bar expands and pushes other content down from the user's field of view.
This update is supported in DHIS version 2.38 or higher with Capture version 100.26.0 or higher.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14008)

**Ask user to create new event when stage is complete:**
Capture app now includes functionality for asking users to create a new event after completing a stage. If the flag for asking the user to create a new stage is checked, users will be prompted to create a new event immediately upon completing the stage. This feature can improve data entry efficiency and reduce human errors. It was previously supported in the old Tracker Capture app and has now been re-implemented in Capture in an improved form.
This feature is supported in DHIS version 2.38 or higher with Capture version 100.21.0 or higher.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13801)

**Create a new TEI when no results match:**
After searching for a tracked entity instance in the Capture app and finding no results, users are now given the option to carry over the search criteria and create a new tracked entity instance. This feature was supported in the old Tracker Capture app and has now been re-implemented in Capture in an improved form.
It is supported in DHIS version 2.38 or higher with Capture version 100.20.0 or higher.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-9666)

**Hide due date:** The Capture app now supports hiding the scheduled date for individual program stages. This feature allows program stages that do not require scheduling or a scheduled date to have those fields hidden, resulting in a cleaner and more streamlined user interface.
This feature is supported in DHIS version 2.38 or higher with Capture version 100.19.0 or higher.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13897)

**Usability improvements:** Several non-functional usability updates have been implemented in the Capture app to provide a better user experience and a smoother look in certain situations. While each change is small, together they provide a better user experience.
These changes are all supported in DHIS2 version 2.38 and above and Capture version 100.29.0 and above includes all these changes.  
[Jira 1](https://dhis2.atlassian.net/browse/DHIS2-12256) | [Jira 2](https://dhis2.atlassian.net/browse/DHIS2-14868) | [Jira 3](https://dhis2.atlassian.net/browse/DHIS2-12337) | [Jira 4](https://dhis2.atlassian.net/browse/DHIS2-13803) | [Jira 5](https://dhis2.atlassian.net/browse/DHIS2-14336) | [Jira 6](https://dhis2.atlassian.net/browse/DHIS2-14125)

**API for downloading files uploaded as tracked entity attributes:** A new API has been created in DHIS2 to allow accessing the file resources that are uploaded as tracked entity attribute values. This feature enables users to use files as tracked entity attributes, such as uploading a birth certificate for a child.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13657)

**API support for downloading tracked entities as CSV from /tracker** DHIS2's `/tracker` endpoint now supports the functionality to download a tracked entity instance directly into a comma-separated value list. This feature is useful for exporting data to other systems that accept CSV.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13620)


## PLATFORM FEATURES

**Aggregate Data Exchange:** The aggregate data exchange service offers the ability to exchange data between instances of DHIS 2, and possibly other software which supports the DHIS 2 data value set JSON format. It also allows for data exchange within a single instance of DHIS 2, for instance for aggregation of tracker data and saving the result as aggregate data.  
The aggregate data exchange service is suitable for use-cases such as:  
Data exchange between an HMIS instance to a data portal or data warehouse instance of DHIS 2.
Data exchange between a DHIS 2 tracker instance with individual data to an aggregate HMIS instance.
Precomputation of tracker data with program indicators saved as aggregate data values.
Data reporting from a national HMIS to a global donor.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-13105) | [Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/data-exchange.html)

**Event Hooks:** The event hook API is a powerful tool that can help you automate your workflows and keep your systems in sync with each other by allowing users to subscribe to two types of events that occur within the DHIS2: metadata events and scheduler events.  
To use the event hook API, you will need to enable it in your DHIS2 configuration file, and then configure the source and target of your event hook, such as webhooks, JMS, and Kafka; you can receive the events and take action in real-time. 
For example, you could set up an event hook that listens for changes to data elements in your metadata, and then sends a webhook to another system to update their records accordingly.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-12194) | [Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/event-hooks.html)

**Multi-select option sets for aggregate data entry:** Users can now configure `MULTI_TEXT` data elements, which allows users to select multiple options for an option set. This feature is currently only added for aggregate data entry.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14481)

**Improvements to Data Integrity:** The Data Integrity API has been improved to handle the growing number of checks. To avoid exceeding the maximum URL length, the following changes have been implemented:
- POST endpoints now accept the list of checks as a request body
- Identifiers have been shortened
- Slow tests have been excluded from wildcard name expansion
- 25 new integrity checks
- Integrity checks for Organisation Units with same name and parent
- Integrity checks for Data Elements belonging to data sets with different periods types  
[Jira 1](https://dhis2.atlassian.net/browse/DHIS2-14506) | [Jira 2](https://dhis2.atlassian.net/browse/DHIS2-14236) | [Jira 3](https://dhis2.atlassian.net/browse/DHIS2-14495) | [Jira 4](https://dhis2.atlassian.net/browse/DHIS2-14451)

**New job for refreshing Materialized view SQL views:** SQL views of type "Materialized view" now has a new Job which can be scheduled to refresh the contents of the SQL view.  
[Jira (Backend)](https://dhis2.atlassian.net/browse/DHIS2-14718) | [Jira (Frontend)](https://dhis2.atlassian.net/browse/DHIS2-15095) | [Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-239/scheduling.html#job-parameters)

**Jobs can now be grouped to run in sequence:** Jobs can be grouped to run in sequence, making it easier to define dependencies between jobs, and also clarify which jobs can be run in parallel. The feature is also soon available in the Scheduler app.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14314) | [Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/scheduling.html#queues)

**Users can no longer be created with case-sensitive usernames:** Existing users can still have the same usernames, with different upper- and lower-case variants, but new users must have a case-insensitive unique username accross all users.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-10886?filter=10404)


### PLATFORM API FEATURES

**Embedded OpenAPI 3 Specification:**
From version 40 onwards, working with the DHIS2 API just got a whole lot easier. The server can now provide a comprehensive OpenAPI document that covers all endpoints, allowing users to quickly and easily understand the capabilities of the API. Both JSON and YAML formats are supported, so you can choose the one that works best for you. And if you want to generate a document for a specific endpoint or a selection of root paths and tags, it's as simple as making a request to the right endpoint. So whether you're a developer, analyst, or data manager, the OpenAPI feature will help you get the most out of DHIS2.  
[Docs](https://docs.dhis2.org/en/develop/core-openapi-specification.html)

**Remove ProgramTrackedEntityAttributeGroup:**  This unused entity was removed from the software, and the relevant database tables, api endpoints and references will no longer be available.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14815)

**New dedicated ping endpoint:** A new endpoint for pinging the server has been added. The new endpoint does not require authentication, extend the user session and uses a low amount of resources.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14531)

**New system info endpoint:** A new endpoint has been added to return information about the current system, including version, revision, build time and system ID.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14822)

**DataStore now returns sharing information:** DataStore keys can be shared in the same way Metadata is shared. With this change, sharing information is now available in the DataStore API: `/api/dataStore/<namespace>/<key>/metaData`  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-14595)

**(Preview) API Routes:** We are introducing a new feature called the Route API, which enables seamless communication with external HTTP gateways or proxies. This feature allows users to extend the functionality of their apps by easily performing GET and POST requests to external services. Users can create routes, execute them, and pass query parameters and request bodies. The Route API supports authentication methods such as HTTP Basic and API Token, and also allows for custom authorities for route execution. This feature provides a simple and effective way to integrate external services into DHIS2 apps.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-12193) | [Docs]()

**(Preview) User impersonation:** Users with the appropriate authority can now impersonate other users. This is primarily used internally in DHIS2 for generating reports at the current time, but will be enhanced in the future to support more usecases. User impersonation is by default disabled in the system.  
[Jira](https://dhis2.atlassian.net/browse/DHIS2-10661)


## RELEASE INFO

|Release Information|Link|
| --- | --- |
|Download release and sample database|https://www.dhis2.org/downloads|
|Documentation|[https://docs.dhis2.org](https://docs.dhis2.org/)|
|Upgrade notes|[Upgrade notes on GitHub](https://github.com/dhis2/dhis2-releases/blob/master/releases/2.40/README.md)|
|Full list of features and bugs|[Release Note](https://github.com/dhis2/dhis2-releases/blob/master/releases/2.40/ReleaseNote-2.40.0.md)|
|Source code on GitHub|https://github.com/dhis2|
|Demo instance|https://play.dhis2.org/40.0.0/|
|Docker image|`docker pull dhis2/core:40.0.0`|
|Docker Hub images|https://hub.docker.com/r/dhis2/core|
|Community forum|https://community.dhis2.org/|