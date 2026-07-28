# PatchedRequestRuleBindingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**uuid** | Option<**uuid::Uuid**> |  | [optional]
**policy_engine_mode** | Option<[**models::PolicyEngineMode**](PolicyEngineMode.md)> |  | [optional]
**rule** | Option<**uuid::Uuid**> |  | [optional]
**target** | Option<**uuid::Uuid**> |  | [optional]
**expiry_pending** | Option<**String**> | How long a request against this binding stays pending before it automatically lapses if not approved or denied. | [optional]
**expiry_granted_max** | Option<**String**> | The maximum duration a grant approved against this binding can last. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


