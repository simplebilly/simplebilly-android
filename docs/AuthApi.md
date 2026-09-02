# AuthApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**acceptInvite**](AuthApi.md#acceptInvite) | **POST** /auth/accept-invite | Accept an invite: create the account (or reuse an existing one) and join the inviting tenant. The invite token proves control of the mailbox.
[**forgotPassword**](AuthApi.md#forgotPassword) | **POST** /auth/forgot-password | Send a password reset email to the user
[**login**](AuthApi.md#login) | **POST** /auth/login | Authenticate a user with email + password (optional TOTP)
[**logout**](AuthApi.md#logout) | **POST** /auth/logout | Log out the current user (kills the assay session)
[**magicLinkLogin**](AuthApi.md#magicLinkLogin) | **POST** /auth/magic-link | Request a magic link login (sends an email with a one-time link)
[**magicLinkVerify**](AuthApi.md#magicLinkVerify) | **POST** /auth/magic-link/verify | Verify a magic link token and log the user in
[**register**](AuthApi.md#register) | **POST** /auth/register | Register a new user account
[**resetPassword**](AuthApi.md#resetPassword) | **POST** /auth/reset-password | Reset the user&#39;s password using a reset token
[**totpEnable**](AuthApi.md#totpEnable) | **POST** /auth/totp/enable | Enable TOTP two-factor authentication by verifying a code
[**totpSetup**](AuthApi.md#totpSetup) | **GET** /auth/totp/setup | Set up TOTP two-factor authentication (generates secret + backup codes)
[**verifyEmail**](AuthApi.md#verifyEmail) | **POST** /auth/verify-email | Verify a user&#39;s email address using a verification token



## acceptInvite

> acceptInvite(acceptInviteRequest)

Accept an invite: create the account (or reuse an existing one) and join the inviting tenant. The invite token proves control of the mailbox.

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
AcceptInviteRequest acceptInviteRequest = new AcceptInviteRequest(); // AcceptInviteRequest | 
try {
    apiInstance.acceptInvite(acceptInviteRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#acceptInvite");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acceptInviteRequest** | [**AcceptInviteRequest**](AcceptInviteRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## forgotPassword

> forgotPassword(forgotPasswordRequest)

Send a password reset email to the user

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
ForgotPasswordRequest forgotPasswordRequest = new ForgotPasswordRequest(); // ForgotPasswordRequest | 
try {
    apiInstance.forgotPassword(forgotPasswordRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#forgotPassword");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **forgotPasswordRequest** | [**ForgotPasswordRequest**](ForgotPasswordRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## login

> AuthResponse login(loginRequest)

Authenticate a user with email + password (optional TOTP)

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
LoginRequest loginRequest = new LoginRequest(); // LoginRequest | 
try {
    AuthResponse result = apiInstance.login(loginRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#login");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **loginRequest** | [**LoginRequest**](LoginRequest.md)|  |

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## logout

> logout()

Log out the current user (kills the assay session)

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
try {
    apiInstance.logout();
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#logout");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## magicLinkLogin

> magicLinkLogin(magicLinkRequest)

Request a magic link login (sends an email with a one-time link)

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
MagicLinkRequest magicLinkRequest = new MagicLinkRequest(); // MagicLinkRequest | 
try {
    apiInstance.magicLinkLogin(magicLinkRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#magicLinkLogin");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **magicLinkRequest** | [**MagicLinkRequest**](MagicLinkRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## magicLinkVerify

> AuthResponse magicLinkVerify(magicLinkVerifyRequest)

Verify a magic link token and log the user in

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
MagicLinkVerifyRequest magicLinkVerifyRequest = new MagicLinkVerifyRequest(); // MagicLinkVerifyRequest | 
try {
    AuthResponse result = apiInstance.magicLinkVerify(magicLinkVerifyRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#magicLinkVerify");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **magicLinkVerifyRequest** | [**MagicLinkVerifyRequest**](MagicLinkVerifyRequest.md)|  |

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## register

> AuthResponse register(registerRequest)

Register a new user account

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
RegisterRequest registerRequest = new RegisterRequest(); // RegisterRequest | 
try {
    AuthResponse result = apiInstance.register(registerRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#register");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registerRequest** | [**RegisterRequest**](RegisterRequest.md)|  |

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## resetPassword

> resetPassword(resetPasswordRequest)

Reset the user&#39;s password using a reset token

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
ResetPasswordRequest resetPasswordRequest = new ResetPasswordRequest(); // ResetPasswordRequest | 
try {
    apiInstance.resetPassword(resetPasswordRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#resetPassword");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **resetPasswordRequest** | [**ResetPasswordRequest**](ResetPasswordRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## totpEnable

> totpEnable(totpEnableRequest)

Enable TOTP two-factor authentication by verifying a code

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
TotpEnableRequest totpEnableRequest = new TotpEnableRequest(); // TotpEnableRequest | 
try {
    apiInstance.totpEnable(totpEnableRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#totpEnable");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **totpEnableRequest** | [**TotpEnableRequest**](TotpEnableRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## totpSetup

> TotpSetupResponse totpSetup()

Set up TOTP two-factor authentication (generates secret + backup codes)

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
try {
    TotpSetupResponse result = apiInstance.totpSetup();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#totpSetup");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**TotpSetupResponse**](TotpSetupResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## verifyEmail

> verifyEmail(verifyEmailRequest)

Verify a user&#39;s email address using a verification token

### Example

```java
// Import classes:
//import org.openapitools.client.api.AuthApi;

AuthApi apiInstance = new AuthApi();
VerifyEmailRequest verifyEmailRequest = new VerifyEmailRequest(); // VerifyEmailRequest | 
try {
    apiInstance.verifyEmail(verifyEmailRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthApi#verifyEmail");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **verifyEmailRequest** | [**VerifyEmailRequest**](VerifyEmailRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

