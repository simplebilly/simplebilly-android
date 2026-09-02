

# Employee

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **String** |  |  [optional]
**backupEmployeeId** | [**UUID**](UUID.md) | References another employee who covers when this employee is absent. |  [optional]
**bic** | **String** |  |  [optional]
**city** | **String** |  |  [optional]
**country** | [**CountryCode**](CountryCode.md) |  |  [optional]
**createdAt** | [**Date**](Date.md) |  |  [optional]
**dateOfBirth** | [**Date**](Date.md) |  |  [optional]
**deletedAt** | [**Date**](Date.md) |  |  [optional]
**departmentId** | [**UUID**](UUID.md) | References the department entity. |  [optional]
**email** | **String** |  |  [optional]
**firstName** | **String** |  |  [optional]
**gender** | [**Gender**](Gender.md) | Gender for pay-transparency reporting: \&quot;male\&quot;, \&quot;female\&quot; or \&quot;diverse\&quot;. |  [optional]
**hireDate** | [**Date**](Date.md) |  |  [optional]
**hourlyCost** | **String** | Hourly cost rate in EUR for labor-cost reporting; when unset the rate is derived from &#x60;monthly_salary / (weekly_hours * 4.33)&#x60;. |  [optional]
**iban** | **String** |  |  [optional]
**id** | [**UUID**](UUID.md) |  |  [optional]
**jobTitle** | **String** |  |  [optional]
**lastLogin** | [**Date**](Date.md) |  |  [optional]
**lastName** | **String** |  |  [optional]
**lastUpdated** | [**Date**](Date.md) |  |  [optional]
**monthlySalary** | **String** | Gross monthly salary in EUR for pay-transparency reporting. |  [optional]
**phone** | **String** |  |  [optional]
**state** | **String** |  |  [optional]
**status** | [**EmployeeStatus**](EmployeeStatus.md) |  |  [optional]
**tenantId** | [**UUID**](UUID.md) |  |  [optional]
**updatedAt** | [**Date**](Date.md) |  |  [optional]
**userId** | [**UUID**](UUID.md) | References the user entity. |  [optional]
**weeklyHours** | **String** | Contractual weekly working hours for pay-transparency normalization. |  [optional]
**zip** | **String** |  |  [optional]




