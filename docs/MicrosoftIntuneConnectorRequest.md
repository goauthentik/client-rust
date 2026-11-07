# MicrosoftIntuneConnectorRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connector_uuid** | Option<**uuid::Uuid**> |  | [optional]
**name** | **String** |  | 
**enabled** | Option<**bool**> |  | [optional]
**client_id** | **String** |  | 
**client_secret** | **String** |  | 
**tenant_id** | **String** |  | 
**certificate_authorities** | Option<**Vec<uuid::Uuid>**> | Certificate authorities which issue device certificates via Intune (Cloud PKI, SCEP or PKCS profiles), used by the endpoint stage to validate certificates. This option has a higher priority than the `client_certificate` option on `Brand`. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


