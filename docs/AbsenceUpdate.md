

# AbsenceUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**absenceType** | [**AbsenceType**](AbsenceType.md) | One of \&quot;vacation\&quot;, \&quot;sick\&quot;, \&quot;sabbatical\&quot;, \&quot;parental\&quot;, \&quot;other\&quot;. |  [optional]
**approvedAt** | [**Date**](Date.md) |  |  [optional]
**approvedBy** | [**UUID**](UUID.md) | References the user entity. |  [optional]
**employeeId** | [**UUID**](UUID.md) | References the employee entity. |  [optional]
**endDate** | [**Date**](Date.md) |  |  [optional]
**notes** | **String** |  |  [optional]
**startDate** | [**Date**](Date.md) |  |  [optional]
**status** | [**AbsenceStatus**](AbsenceStatus.md) | One of \&quot;pending\&quot;, \&quot;approved\&quot;, \&quot;rejected\&quot;, \&quot;cancelled\&quot;. |  [optional]




