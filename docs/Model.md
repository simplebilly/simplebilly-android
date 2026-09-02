

# Model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**backupCodes** | **List&lt;String&gt;** |  | 
**createdAt** | [**Date**](Date.md) |  | 
**deletedAt** | [**Date**](Date.md) |  |  [optional]
**email** | **String** |  | 
**emailVerified** | **Boolean** |  | 
**id** | [**UUID**](UUID.md) |  | 
**isActive** | **Boolean** |  | 
**isTotpEnabled** | **Boolean** |  | 
**lastLogin** | [**Date**](Date.md) |  |  [optional]
**name** | **String** |  | 
**oauthId** | **String** |  |  [optional]
**oauthProvider** | **String** |  |  [optional]
**passwordChangedAt** | [**Date**](Date.md) | Set on password change; auth/refresh tokens issued before this timestamp are rejected by the auth middleware. |  [optional]
**passwordHash** | **String** |  | 
**picture** | **String** |  |  [optional]
**privacyAcceptedAt** | [**Date**](Date.md) | When the user accepted the data privacy policy (GDPR consent record). |  [optional]
**totpSecret** | **String** |  |  [optional]
**updatedAt** | [**Date**](Date.md) |  | 




