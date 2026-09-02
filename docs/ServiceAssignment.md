

# ServiceAssignment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employeeId** | [**UUID**](UUID.md) | References the employees entity. |  [optional]
**jobId** | [**UUID**](UUID.md) | References the service_jobs entity. |  [optional]
**notes** | **String** |  |  [optional]
**scheduledDate** | [**Date**](Date.md) | Work day the assignment is scheduled for. |  [optional]
**scheduledEnd** | **String** | Planned end time of the assignment. |  [optional]
**scheduledStart** | **String** | Planned start time of the assignment. |  [optional]
**status** | [**ServiceAssignmentStatus**](ServiceAssignmentStatus.md) | Assignment lifecycle status: \&quot;planned\&quot;, \&quot;confirmed\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot; or \&quot;cancelled\&quot;. |  [optional]




