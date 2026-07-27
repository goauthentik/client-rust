# UserOffboarding

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [readonly]
**user** | **i32** |  | 
**user_obj** | [**models::PartialUser**](PartialUser.md) |  | [readonly]
**scheduled_at** | **chrono::DateTime<chrono::FixedOffset>** | Absolute time at which the offboarding action is executed. | 
**action** | Option<[**models::OffboardingActionEnum**](OffboardingActionEnum.md)> |  | [optional]
**revoke_sessions** | Option<**bool**> | Revoke all of the user's sessions when offboarding. | [optional]
**revoke_tokens** | Option<**bool**> | Revoke all of the user's tokens when offboarding. | [optional]
**status** | [**models::OffboardingStatusEnum**](OffboardingStatusEnum.md) |  | [readonly]
**created_by_obj** | [**models::PartialUser**](PartialUser.md) |  | [readonly]
**created_at** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**executed_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


