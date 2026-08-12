# PatchedSourceStageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> |  | [optional]
**source** | Option<**uuid::Uuid**> |  | [optional]
**resume_timeout** | Option<**String**> | Amount of time a user can take to return from the source to continue the flow (Format: hours=-1;minutes=-2;seconds=-3) | [optional]
**resume_on_match_failures** | Option<[**Vec<models::ResumeOnMatchFailuresEnum>**](ResumeOnMatchFailuresEnum.md)> | Source matching failure reasons for which the flow should resume. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


