# ObjectAttribute

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pk** | **uuid::Uuid** |  | [readonly]
**object_type** | **String** |  | 
**object_type_obj** | [**models::ContentType**](ContentType.md) |  | [readonly]
**enabled** | Option<**bool**> |  | [optional][default to true]
**created** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**key** | **String** |  | 
**label** | **String** |  | 
**last_updated** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**regex** | Option<**String**> |  | [optional]
**r#type** | [**models::ObjectAttributeTypeEnum**](ObjectAttributeTypeEnum.md) |  | 
**group** | Option<**String**> |  | [optional]
**managed** | Option<**String**> | Objects that are managed by authentik. These objects are created and updated automatically. This flag only indicates that an object can be overwritten by migrations. You can still modify the objects via the API, but expect changes to be overwritten in a later update. | [optional]
**is_unique** | Option<**bool**> |  | [optional]
**is_required** | Option<**bool**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


