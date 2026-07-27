# UserOffboardingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | **i32** |  | 
**scheduled_at** | **chrono::DateTime<chrono::FixedOffset>** | Absolute time at which the offboarding action is executed. | 
**action** | Option<[**models::OffboardingActionEnum**](OffboardingActionEnum.md)> |  | [optional]
**revoke_sessions** | Option<**bool**> | Revoke all of the user's sessions when offboarding. | [optional]
**revoke_tokens** | Option<**bool**> | Revoke all of the user's tokens when offboarding. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


