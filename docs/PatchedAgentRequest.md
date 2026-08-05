# PatchedAgentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | Option<**String**> | Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only. | [optional]
**name** | Option<**String**> | User's display name. | [optional]
**is_active** | Option<**bool**> | Designates whether this user should be treated as active. Unselect this instead of deleting accounts. | [optional]
**last_login** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**email** | Option<**String**> |  | [optional]
**attributes** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**expiring** | Option<**bool**> |  | [optional]
**expires** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


