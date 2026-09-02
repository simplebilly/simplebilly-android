

# Job

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attempts** | **Integer** |  |  [optional]
**jobType** | **String** | Discriminator the worker dispatches on (e.g. \&quot;webhook.deliver\&quot;). | 
**maxAttempts** | **Integer** |  | 
**payload** | [**OasAnyTypeNotMapped**](.md) |  |  [optional]
**runAt** | [**Date**](Date.md) | Earliest execution time; None &#x3D; run now. |  [optional]
**status** | [**JobStatus**](JobStatus.md) | pending | running | done | failed | 




