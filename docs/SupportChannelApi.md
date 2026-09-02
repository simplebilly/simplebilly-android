# SupportChannelApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createChannelApi**](SupportChannelApi.md#createChannelApi) | **POST** /api/v1/support/channels | 
[**deleteChannelApi**](SupportChannelApi.md#deleteChannelApi) | **DELETE** /api/v1/support/channels/{channel_id} | 
[**listChannelsApi**](SupportChannelApi.md#listChannelsApi) | **GET** /api/v1/support/channels | 
[**updateChannelApi**](SupportChannelApi.md#updateChannelApi) | **PUT** /api/v1/support/channels/{channel_id} | 



## createChannelApi

> SupportChannel createChannelApi(createChannelDto)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportChannelApi;

SupportChannelApi apiInstance = new SupportChannelApi();
CreateChannelDto createChannelDto = new CreateChannelDto(); // CreateChannelDto | 
try {
    SupportChannel result = apiInstance.createChannelApi(createChannelDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportChannelApi#createChannelApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createChannelDto** | [**CreateChannelDto**](CreateChannelDto.md)|  |

### Return type

[**SupportChannel**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteChannelApi

> deleteChannelApi(channelId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportChannelApi;

SupportChannelApi apiInstance = new SupportChannelApi();
UUID channelId = null; // UUID | 
try {
    apiInstance.deleteChannelApi(channelId);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportChannelApi#deleteChannelApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channelId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## listChannelsApi

> List&lt;SupportChannel&gt; listChannelsApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportChannelApi;

SupportChannelApi apiInstance = new SupportChannelApi();
try {
    List<SupportChannel> result = apiInstance.listChannelsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportChannelApi#listChannelsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;SupportChannel&gt;**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateChannelApi

> SupportChannel updateChannelApi(channelId, updateChannelDto)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportChannelApi;

SupportChannelApi apiInstance = new SupportChannelApi();
UUID channelId = null; // UUID | 
UpdateChannelDto updateChannelDto = new UpdateChannelDto(); // UpdateChannelDto | 
try {
    SupportChannel result = apiInstance.updateChannelApi(channelId, updateChannelDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportChannelApi#updateChannelApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channelId** | **UUID**|  | [default to null]
 **updateChannelDto** | [**UpdateChannelDto**](UpdateChannelDto.md)|  |

### Return type

[**SupportChannel**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

