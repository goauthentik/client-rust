# PatchedMicrosoftIntuneConnectorRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connector_uuid** | Option<**uuid::Uuid**> |  | [optional]
**name** | Option<**String**> |  | [optional]
**enabled** | Option<**bool**> |  | [optional]
**client_id** | Option<**String**> |  | [optional]
**client_secret** | Option<**String**> |  | [optional]
**tenant_id** | Option<**String**> |  | [optional]
**certificate_authorities** | Option<**Vec<uuid::Uuid>**> | Certificate authorities which issue device certificates via Intune (Cloud PKI, SCEP or PKCS profiles), used by the endpoint stage to validate certificates. This option has a higher priority than the `client_certificate` option on `Brand`. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


