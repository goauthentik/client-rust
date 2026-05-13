# Event

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pk** | **uuid::Uuid** |  | [readonly]
**user** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**action** | [**models::EventActions**](EventActions.md) |  | 
**app** | **String** |  | 
**context** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**client_ip** | Option<**String**> |  | [optional]
**created** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**expires** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**brand** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


