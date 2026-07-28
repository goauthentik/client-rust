# RequestRuleBinding

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**uuid** | Option<**uuid::Uuid**> |  | [optional]
**pbm_uuid** | **uuid::Uuid** |  | [readonly]
**policy_engine_mode** | Option<[**models::PolicyEngineMode**](PolicyEngineMode.md)> |  | [optional]
**rule** | **uuid::Uuid** |  | 
**rule_obj** | [**models::RequestRule**](RequestRule.md) |  | [readonly]
**target** | **uuid::Uuid** |  | 
**related** | **Vec<uuid::Uuid>** |  | [readonly]
**related_obj** | [**Vec<models::RelatedTarget>**](RelatedTarget.md) |  | [readonly]
**expiry_pending** | Option<**String**> | How long a request against this binding stays pending before it automatically lapses if not approved or denied. | [optional]
**expiry_granted_max** | Option<**String**> | The maximum duration a grant approved against this binding can last. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


