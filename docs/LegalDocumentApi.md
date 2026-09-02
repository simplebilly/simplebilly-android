# LegalDocumentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getLegalDocuments**](LegalDocumentApi.md#getLegalDocuments) | **GET** /api/v1/legal/documents | List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.
[**resetLegalDocuments**](LegalDocumentApi.md#resetLegalDocuments) | **POST** /api/v1/legal/documents/reset | Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.
[**upsertLegalDocuments**](LegalDocumentApi.md#upsertLegalDocuments) | **PUT** /api/v1/legal/documents | Upsert legal documents per (doc_type, lang). Returns the full tenant list.



## getLegalDocuments

> List&lt;LegalDocument&gt; getLegalDocuments()

List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.

### Example

```java
// Import classes:
//import org.openapitools.client.api.LegalDocumentApi;

LegalDocumentApi apiInstance = new LegalDocumentApi();
try {
    List<LegalDocument> result = apiInstance.getLegalDocuments();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LegalDocumentApi#getLegalDocuments");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;LegalDocument&gt;**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## resetLegalDocuments

> List&lt;LegalDocument&gt; resetLegalDocuments(legalDocumentReset)

Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.

### Example

```java
// Import classes:
//import org.openapitools.client.api.LegalDocumentApi;

LegalDocumentApi apiInstance = new LegalDocumentApi();
LegalDocumentReset legalDocumentReset = new LegalDocumentReset(); // LegalDocumentReset | 
try {
    List<LegalDocument> result = apiInstance.resetLegalDocuments(legalDocumentReset);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LegalDocumentApi#resetLegalDocuments");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **legalDocumentReset** | [**LegalDocumentReset**](LegalDocumentReset.md)|  |

### Return type

[**List&lt;LegalDocument&gt;**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## upsertLegalDocuments

> List&lt;LegalDocument&gt; upsertLegalDocuments(legalDocumentUpsert)

Upsert legal documents per (doc_type, lang). Returns the full tenant list.

### Example

```java
// Import classes:
//import org.openapitools.client.api.LegalDocumentApi;

LegalDocumentApi apiInstance = new LegalDocumentApi();
List<LegalDocumentUpsert> legalDocumentUpsert = Arrays.asList(new LegalDocumentUpsert()); // List<LegalDocumentUpsert> | 
try {
    List<LegalDocument> result = apiInstance.upsertLegalDocuments(legalDocumentUpsert);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LegalDocumentApi#upsertLegalDocuments");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **legalDocumentUpsert** | [**List&lt;LegalDocumentUpsert&gt;**](LegalDocumentUpsert.md)|  |

### Return type

[**List&lt;LegalDocument&gt;**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

