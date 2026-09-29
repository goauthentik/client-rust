# PatchedRacProviderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> |  | [optional]
**authentication_flow** | Option<**uuid::Uuid**> | Flow used for authentication when the associated application is accessed by an un-authenticated user. | [optional]
**authorization_flow** | Option<**uuid::Uuid**> | Flow used when authorizing this provider. | [optional]
**property_mappings** | Option<**Vec<uuid::Uuid>**> |  | [optional]
**settings** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**access_group** | Option<**uuid::Uuid**> | Only devices in this access group can be accessed through this provider. When left empty, every device the user has access to can be accessed. | [optional]
**maximum_connections** | Option<**i32**> | Maximum concurrent connections to a single device. Can be set to -1 to disable the limit. | [optional]
**auth_mode** | Option<[**models::RacProviderAuthModeEnum**](RACProviderAuthModeEnum.md)> |  | [optional]
**connection_expiry** | Option<**String**> | Determines how long a session lasts. Default of 0 means that the sessions lasts until the browser is closed. (Format: hours=-1;minutes=-2;seconds=-3) | [optional]
**delete_token_on_disconnect** | Option<**bool**> | When set to true, connection tokens will be deleted upon disconnect. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


