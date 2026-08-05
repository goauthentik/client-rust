# Agent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pk** | **i32** |  | [readonly]
**username** | **String** | Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only. | 
**name** | **String** | User's display name. | 
**is_active** | Option<**bool**> | Designates whether this user should be treated as active. Unselect this instead of deleting accounts. | [optional]
**last_login** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**email** | Option<**String**> |  | [optional]
**attributes** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**uid** | **String** |  | [readonly]
**uuid** | **uuid::Uuid** |  | [readonly]
**expiring** | Option<**bool**> |  | [optional]
**expires** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**parent** | [**models::PartialUser**](PartialUser.md) |  | [readonly]
**policy_behavior** | [**models::PolicyBehaviorEnum**](PolicyBehaviorEnum.md) |  | [readonly]
**token_identifier** | Option<**String**> | Identifier of the agent's API token, so its key can be retrieved/copied later. | [readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


