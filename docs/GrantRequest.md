# GrantRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**created_by** | [**models::PartialUser**](PartialUser.md) |  | [readonly]
**requester_data** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**fulfiller_data** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**revoked_by** | [**models::PartialUser**](PartialUser.md) |  | [readonly]
**is_active** | **bool** |  | [readonly]
**expires** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**status** | [**models::RequestStatus**](RequestStatus.md) |  | [readonly]
**targets** | **Vec<uuid::Uuid>** |  | [readonly]
**target_objs** | [**Vec<models::RequestableTarget>**](RequestableTarget.md) |  | [readonly]
**uuid** | Option<**uuid::Uuid**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


