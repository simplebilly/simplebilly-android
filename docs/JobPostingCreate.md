

# JobPostingCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **String** |  |  [optional]
**department** | **String** |  |  [optional]
**description** | **String** | What the job is; markdown/HTML. | 
**employmentType** | [**EmploymentType**](EmploymentType.md) | full_time | part_time | contract | internship | temporary |  [optional]
**location** | **String** |  |  [optional]
**remote** | **Boolean** |  | 
**requiredSkills** | [**OasAnyTypeNotMapped**](.md) | List of required skill names (JSON array of strings). | 
**requirements** | **String** | Structured profile of the required candidate (skills, experience). |  [optional]
**salaryMax** | **Integer** |  |  [optional]
**salaryMin** | **Integer** |  |  [optional]
**status** | [**JobPostingStatus**](JobPostingStatus.md) | draft | published | closed | 
**title** | **String** |  | 




