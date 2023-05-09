# 2.41 Upgrade Notes

- **Breaking change in Dashboard App**: in 2.40 and older versions, Users can view Dashboard content even without `METADATA_READ` permission to all metadata objects linked to DashboardItems. That is possible because of a loophole in our web api which allows any User to see details of any metadata object if the `uid` is known. This loophole has been causing issues for a long time so we decided to remove it in 2.41. As a result, many Users will not be able to view Dashboards because they don't have enough `METADATA_READ` permission of the Dashboard content. In order to fix it, the System Administrator or the Dashboard owner can make use of the feature [Cascade sharing for Dashboard](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-237/sharing.html#cascade-sharing-for-dashboard) to grant required permissions to affected Users.
- **Legacy Sharing properties are removed**: from 2.36 a new `sharing` property has been introduced in order to replace the legacy sharing properties userAccesses, userGroupAccesses, publicAccess, externalAccess. In order to keep the web api backward compability we have been supported both new and legacy properties our web api and all related features. However, in order to implement new features and keep the code base clean we need to remove the legacy format in 2.41. So from this version, you will not get those properties returned from our web api : `userAccesses`, `userGroupAccesses`, `publicAccess`, `externalAccess`. Instead, those properties can be accessed in new `sharing` properties as documented [here](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-237/sharing.html#new-sharing-object).