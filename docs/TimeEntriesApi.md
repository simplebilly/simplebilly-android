# TimeEntriesApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**clockInTimeEntry**](TimeEntriesApi.md#clockInTimeEntry) | **POST** /api/v1/time-entries | Clock in for the authenticated user (resolved via their employee profile).
[**clockOutTimeEntry**](TimeEntriesApi.md#clockOutTimeEntry) | **PATCH** /api/v1/time-entries/{id} | Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.
[**getLaborCosts**](TimeEntriesApi.md#getLaborCosts) | **GET** /api/v1/labor-costs | Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate.
[**listTimeEntries**](TimeEntriesApi.md#listTimeEntries) | **GET** /api/v1/time-entries | List time entries with optional date-range / active / employee filters.



## clockInTimeEntry

> TimeEntryDto clockInTimeEntry(timeEntryClockIn)

Clock in for the authenticated user (resolved via their employee profile).

### Example

```java
// Import classes:
//import org.openapitools.client.api.TimeEntriesApi;

TimeEntriesApi apiInstance = new TimeEntriesApi();
TimeEntryClockIn timeEntryClockIn = new TimeEntryClockIn(); // TimeEntryClockIn | 
try {
    TimeEntryDto result = apiInstance.clockInTimeEntry(timeEntryClockIn);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TimeEntriesApi#clockInTimeEntry");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **timeEntryClockIn** | [**TimeEntryClockIn**](TimeEntryClockIn.md)|  |

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## clockOutTimeEntry

> TimeEntryDto clockOutTimeEntry(id, timeEntryClockOut)

Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.

### Example

```java
// Import classes:
//import org.openapitools.client.api.TimeEntriesApi;

TimeEntriesApi apiInstance = new TimeEntriesApi();
UUID id = null; // UUID | 
TimeEntryClockOut timeEntryClockOut = new TimeEntryClockOut(); // TimeEntryClockOut | 
try {
    TimeEntryDto result = apiInstance.clockOutTimeEntry(id, timeEntryClockOut);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TimeEntriesApi#clockOutTimeEntry");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **timeEntryClockOut** | [**TimeEntryClockOut**](TimeEntryClockOut.md)|  |

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getLaborCosts

> List&lt;LaborCostRow&gt; getLaborCosts(from, to, groupBy)

Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate.

### Example

```java
// Import classes:
//import org.openapitools.client.api.TimeEntriesApi;

TimeEntriesApi apiInstance = new TimeEntriesApi();
Date from = null; // Date | 
Date to = null; // Date | 
String groupBy = null; // String | One of \"employee\", \"order\" or \"day\".
try {
    List<LaborCostRow> result = apiInstance.getLaborCosts(from, to, groupBy);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TimeEntriesApi#getLaborCosts");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from** | **Date**|  | [default to null]
 **to** | **Date**|  | [default to null]
 **groupBy** | **String**| One of \&quot;employee\&quot;, \&quot;order\&quot; or \&quot;day\&quot;. | [default to null]

### Return type

[**List&lt;LaborCostRow&gt;**](LaborCostRow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listTimeEntries

> List&lt;TimeEntryDto&gt; listTimeEntries(from, to, active, employeeId)

List time entries with optional date-range / active / employee filters.

### Example

```java
// Import classes:
//import org.openapitools.client.api.TimeEntriesApi;

TimeEntriesApi apiInstance = new TimeEntriesApi();
Date from = null; // Date | 
Date to = null; // Date | 
Boolean active = null; // Boolean | Only currently running shifts (clock_in set, clock_out null).
UUID employeeId = null; // UUID | 
try {
    List<TimeEntryDto> result = apiInstance.listTimeEntries(from, to, active, employeeId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TimeEntriesApi#listTimeEntries");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from** | **Date**|  | [optional] [default to null]
 **to** | **Date**|  | [optional] [default to null]
 **active** | **Boolean**| Only currently running shifts (clock_in set, clock_out null). | [optional] [default to null]
 **employeeId** | **UUID**|  | [optional] [default to null]

### Return type

[**List&lt;TimeEntryDto&gt;**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

