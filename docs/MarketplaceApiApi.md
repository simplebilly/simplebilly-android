# MarketplaceApiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createConnectionApi**](MarketplaceApiApi.md#createConnectionApi) | **POST** /api/v1/marketplace/connections | Create a new connection (for API-key based platforms)
[**deleteConnectionApi**](MarketplaceApiApi.md#deleteConnectionApi) | **DELETE** /api/v1/marketplace/connections/{connection_id} | Soft-delete a connection
[**getConnectionApi**](MarketplaceApiApi.md#getConnectionApi) | **GET** /api/v1/marketplace/connections/{connection_id} | Get a single connection
[**getSyncDirectionApi**](MarketplaceApiApi.md#getSyncDirectionApi) | **GET** /api/v1/marketplace/connections/{connection_id}/directions | Get current sync direction configuration for a connection
[**getSyncLogsApi**](MarketplaceApiApi.md#getSyncLogsApi) | **GET** /api/v1/marketplace/connections/{connection_id}/logs | Get sync logs for a connection
[**listConnectionsApi**](MarketplaceApiApi.md#listConnectionsApi) | **GET** /api/v1/marketplace/connections | List connections for the current tenant
[**listPlatformsApi**](MarketplaceApiApi.md#listPlatformsApi) | **GET** /api/v1/marketplace/platforms | List all supported platforms
[**oauthAuthorizeApi**](MarketplaceApiApi.md#oauthAuthorizeApi) | **POST** /api/v1/marketplace/oauth/authorize | OAuth: initiate authorization flow
[**oauthCallbackApi**](MarketplaceApiApi.md#oauthCallbackApi) | **POST** /api/v1/marketplace/oauth/callback | OAuth: handle callback after authorization
[**triggerSyncApi**](MarketplaceApiApi.md#triggerSyncApi) | **POST** /api/v1/marketplace/connections/{connection_id}/sync | Trigger sync for a connection
[**updateConnectionApi**](MarketplaceApiApi.md#updateConnectionApi) | **PUT** /api/v1/marketplace/connections/{connection_id} | Update a connection
[**updateSyncDirectionApi**](MarketplaceApiApi.md#updateSyncDirectionApi) | **PUT** /api/v1/marketplace/connections/{connection_id}/directions | Update per-entity sync direction configuration for a connection
[**webhookReceiverApi**](MarketplaceApiApi.md#webhookReceiverApi) | **POST** /api/v1/marketplace/webhook/{platform}/{connection_id} | Webhook receiver



## createConnectionApi

> MarketplaceConnection createConnectionApi(createConnectionRequest)

Create a new connection (for API-key based platforms)

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
CreateConnectionRequest createConnectionRequest = new CreateConnectionRequest(); // CreateConnectionRequest | 
try {
    MarketplaceConnection result = apiInstance.createConnectionApi(createConnectionRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#createConnectionApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createConnectionRequest** | [**CreateConnectionRequest**](CreateConnectionRequest.md)|  |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteConnectionApi

> deleteConnectionApi(connectionId)

Soft-delete a connection

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String connectionId = null; // String | 
try {
    apiInstance.deleteConnectionApi(connectionId);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#deleteConnectionApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connectionId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getConnectionApi

> MarketplaceConnection getConnectionApi(connectionId)

Get a single connection

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String connectionId = null; // String | 
try {
    MarketplaceConnection result = apiInstance.getConnectionApi(connectionId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#getConnectionApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connectionId** | **String**|  | [default to null]

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSyncDirectionApi

> getSyncDirectionApi(connectionId)

Get current sync direction configuration for a connection

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String connectionId = null; // String | 
try {
    apiInstance.getSyncDirectionApi(connectionId);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#getSyncDirectionApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connectionId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getSyncLogsApi

> List&lt;SyncLog&gt; getSyncLogsApi(connectionId)

Get sync logs for a connection

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String connectionId = null; // String | 
try {
    List<SyncLog> result = apiInstance.getSyncLogsApi(connectionId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#getSyncLogsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connectionId** | **String**|  | [default to null]

### Return type

[**List&lt;SyncLog&gt;**](SyncLog.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listConnectionsApi

> List&lt;MarketplaceConnection&gt; listConnectionsApi()

List connections for the current tenant

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
try {
    List<MarketplaceConnection> result = apiInstance.listConnectionsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#listConnectionsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;MarketplaceConnection&gt;**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPlatformsApi

> List&lt;PlatformInfo&gt; listPlatformsApi()

List all supported platforms

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
try {
    List<PlatformInfo> result = apiInstance.listPlatformsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#listPlatformsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;PlatformInfo&gt;**](PlatformInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## oauthAuthorizeApi

> OAuthAuthorizeResponse oauthAuthorizeApi(oAuthAuthorizeRequest)

OAuth: initiate authorization flow

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
OAuthAuthorizeRequest oAuthAuthorizeRequest = new OAuthAuthorizeRequest(); // OAuthAuthorizeRequest | 
try {
    OAuthAuthorizeResponse result = apiInstance.oauthAuthorizeApi(oAuthAuthorizeRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#oauthAuthorizeApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oAuthAuthorizeRequest** | [**OAuthAuthorizeRequest**](OAuthAuthorizeRequest.md)|  |

### Return type

[**OAuthAuthorizeResponse**](OAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## oauthCallbackApi

> MarketplaceConnection oauthCallbackApi(oAuthCallbackRequest)

OAuth: handle callback after authorization

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
OAuthCallbackRequest oAuthCallbackRequest = new OAuthCallbackRequest(); // OAuthCallbackRequest | 
try {
    MarketplaceConnection result = apiInstance.oauthCallbackApi(oAuthCallbackRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#oauthCallbackApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oAuthCallbackRequest** | [**OAuthCallbackRequest**](OAuthCallbackRequest.md)|  |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## triggerSyncApi

> SyncSummary triggerSyncApi(connectionId, syncType, direction)

Trigger sync for a connection

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String connectionId = null; // String | 
String syncType = null; // String | 
String direction = null; // String | 
try {
    SyncSummary result = apiInstance.triggerSyncApi(connectionId, syncType, direction);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#triggerSyncApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connectionId** | **String**|  | [default to null]
 **syncType** | **String**|  | [optional] [default to null]
 **direction** | **String**|  | [optional] [default to null]

### Return type

[**SyncSummary**](SyncSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateConnectionApi

> MarketplaceConnection updateConnectionApi(connectionId, updateConnectionRequest)

Update a connection

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String connectionId = null; // String | 
UpdateConnectionRequest updateConnectionRequest = new UpdateConnectionRequest(); // UpdateConnectionRequest | 
try {
    MarketplaceConnection result = apiInstance.updateConnectionApi(connectionId, updateConnectionRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#updateConnectionApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connectionId** | **String**|  | [default to null]
 **updateConnectionRequest** | [**UpdateConnectionRequest**](UpdateConnectionRequest.md)|  |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateSyncDirectionApi

> updateSyncDirectionApi(connectionId, updateSyncDirectionRequest)

Update per-entity sync direction configuration for a connection

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String connectionId = null; // String | 
UpdateSyncDirectionRequest updateSyncDirectionRequest = new UpdateSyncDirectionRequest(); // UpdateSyncDirectionRequest | 
try {
    apiInstance.updateSyncDirectionApi(connectionId, updateSyncDirectionRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#updateSyncDirectionApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connectionId** | **String**|  | [default to null]
 **updateSyncDirectionRequest** | [**UpdateSyncDirectionRequest**](UpdateSyncDirectionRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## webhookReceiverApi

> webhookReceiverApi(platform, connectionId)

Webhook receiver

### Example

```java
// Import classes:
//import org.openapitools.client.api.MarketplaceApiApi;

MarketplaceApiApi apiInstance = new MarketplaceApiApi();
String platform = null; // String | 
String connectionId = null; // String | 
try {
    apiInstance.webhookReceiverApi(platform, connectionId);
} catch (ApiException e) {
    System.err.println("Exception when calling MarketplaceApiApi#webhookReceiverApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **platform** | **String**|  | [default to null]
 **connectionId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

