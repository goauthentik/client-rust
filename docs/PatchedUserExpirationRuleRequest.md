# PatchedUserExpirationRuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pk** | Option<**uuid::Uuid**> |  | [optional]
**name** | Option<**String**> |  | [optional]
**enabled** | Option<**bool**> |  | [optional]
**activity_basis** | Option<[**models::ActivityBasisEnum**](ActivityBasisEnum.md)> | Measure inactivity from the last login or successful user activity. | [optional]
**group** | Option<**uuid::Uuid**> | Only expire members of this group (including descendant groups). Leave empty to apply to every user. | [optional]
**user_types** | Option<[**Vec<models::UserTypeEnum>**](UserTypeEnum.md)> | Only expire users of these types. Service accounts are excluded by default. | [optional]
**inactivity_duration** | Option<**String**> | How long a user may be inactive before they are expired. | [optional]
**action** | Option<[**models::OffboardingActionEnum**](OffboardingActionEnum.md)> |  | [optional]
**revoke_sessions** | Option<**bool**> |  | [optional]
**revoke_tokens** | Option<**bool**> |  | [optional]
**warn_before** | Option<**String**> | Schedule the offboarding and notify the user this long before they expire. Leave empty to expire users without warning. | [optional]
**notification_transports** | Option<**Vec<uuid::Uuid>**> | Select which transports should be used to warn the user. If none are selected, the notification will only be shown in the authentik UI. | [optional]
**exclude_superusers** | Option<**bool**> | Never expire members of a superuser group. | [optional]
**policy_engine_mode** | Option<[**models::PolicyEngineMode**](PolicyEngineMode.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


