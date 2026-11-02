# PasswordStage

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
**backends** | [**Vec<models::BackendsEnum>**](BackendsEnum.md) | Selection of backends to test the password against. | 
**configure_flow** | Option<**uuid::Uuid**> | Flow used by an authenticated user to configure this Stage. If empty, user will not be able to configure this stage. | [optional]
**failed_attempts_before_cancel** | Option<**i32**> | How many attempts a user has before the flow is canceled. This only cancels the flow, it does not lock the user's password. | [optional]
**failed_attempts_before_lockout** | Option<**u32**> | How many consecutive failed attempts lock the user's password until an administrator unlocks it. Set to 0 to never lock. | [optional]
**last_attempt_warning_message** | Option<**String**> | Warning shown when the user has one password attempt remaining. Leave blank to show no warning. | [optional]
**lockout_message** | Option<**String**> | Message shown when the user's password has been locked. Leave blank to show a generic authentication error. | [optional]
**allow_show_password** | Option<**bool**> | When enabled, provides a 'show password' button with the password input field. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


