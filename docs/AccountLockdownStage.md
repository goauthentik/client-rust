# AccountLockdownStage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pk** | **uuid::Uuid** |  | [readonly]
**name** | **String** |  | 
**component** | **String** | Get object type so that we know how to edit the object | [readonly]
**verbose_name** | **String** | Return object's verbose_name | [readonly]
**verbose_name_plural** | **String** | Return object's plural verbose_name | [readonly]
**meta_model_name** | **String** | Return internal model name | [readonly]
**flow_set** | [**Vec<models::FlowSet>**](FlowSet.md) |  | [readonly]
**deactivate_user** | Option<**bool**> | Deactivate the user account (set is_active to False) | [optional]
**set_unusable_password** | Option<**bool**> | Set an unusable password for the user | [optional]
**delete_sessions** | Option<**bool**> | Delete all active sessions for the user | [optional]
**revoke_tokens** | Option<**bool**> | Revoke all tokens for the user (API, app password, recovery, verification, OAuth) | [optional]
**self_service_completion_flow** | Option<**uuid::Uuid**> | Flow to redirect users to after self-service lockdown. This flow should not require authentication since the user's session is deleted. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


