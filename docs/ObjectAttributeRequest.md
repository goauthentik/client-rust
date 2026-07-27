# ObjectAttributeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**object_type** | **String** |  | 
**enabled** | Option<**bool**> |  | [optional][default to true]
**key** | **String** |  | 
**label** | **String** |  | 
**regex** | Option<**String**> |  | [optional]
**r#type** | [**models::ObjectAttributeTypeEnum**](ObjectAttributeTypeEnum.md) |  | 
**group** | Option<**String**> |  | [optional]
**managed** | Option<**String**> | Objects that are managed by authentik. These objects are created and updated automatically. This flag only indicates that an object can be overwritten by migrations. You can still modify the objects via the API, but expect changes to be overwritten in a later update. | [optional]
**is_unique** | Option<**bool**> |  | [optional]
**is_required** | Option<**bool**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


