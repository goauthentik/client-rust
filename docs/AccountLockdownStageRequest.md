# AccountLockdownStageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** |  | 
**deactivate_user** | Option<**bool**> | Deactivate the user account (set is_active to False) | [optional]
**set_unusable_password** | Option<**bool**> | Set an unusable password for the user | [optional]
**delete_sessions** | Option<**bool**> | Delete all active sessions for the user | [optional]
**revoke_tokens** | Option<**bool**> | Revoke all tokens for the user (API, app password, recovery, verification, OAuth) | [optional]
**self_service_completion_flow** | Option<**uuid::Uuid**> | Flow to redirect users to after self-service lockdown. This flow should not require authentication since the user's session is deleted. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


