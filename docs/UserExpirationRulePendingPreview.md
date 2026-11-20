# UserExpirationRulePendingPreview

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [readonly]
**user** | [**models::UserExpirationRuleUser**](UserExpirationRuleUser.md) |  | [readonly]
**previous_action** | [**models::OffboardingActionEnum**](OffboardingActionEnum.md) |  | [readonly]
**action** | Option<[**models::OffboardingActionEnum**](OffboardingActionEnum.md)> |  | [readonly]
**previous_scheduled_at** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**scheduled_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [readonly]
**previous_revoke_sessions** | **bool** |  | [readonly]
**revoke_sessions** | Option<**bool**> |  | [readonly]
**previous_revoke_tokens** | **bool** |  | [readonly]
**revoke_tokens** | Option<**bool**> |  | [readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


