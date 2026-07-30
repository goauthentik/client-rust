# OAuth2DynamicClientRegistrationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider** | **i32** |  | 
**default_application_group** | Option<**String**> | Group to assign to automatically created applications. | [optional]
**override_authorization_flow** | Option<**uuid::Uuid**> | Authorization flow applied to dynamically registered clients. | [optional]
**override_invalidation_flow** | Option<**uuid::Uuid**> |  | [optional]
**override_property_mappings** | Option<**Vec<uuid::Uuid>**> | Scope mappings applied to dynamically registered clients. | [optional]
**access_token_validity** | Option<**String**> | Maximum access token validity for registered clients (Format: hours=1;minutes=2;seconds=3). | [optional]
**refresh_token_validity** | Option<**String**> | Maximum refresh token validity for registered clients (Format: hours=1;minutes=2;seconds=3). | [optional]
**allowed_grant_types** | Option<[**Vec<models::GrantTypeEnum>**](GrantTypeEnum.md)> | If empty, all grant types are allowed. | [optional]
**policy_engine_mode** | Option<[**models::PolicyEngineMode**](PolicyEngineMode.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


