# MicrosoftIntuneConnector

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connector_uuid** | Option<**uuid::Uuid**> |  | [optional]
**name** | **String** |  | 
**enabled** | Option<**bool**> |  | [optional]
**component** | **String** | Get object component so that we know how to edit the object | [readonly]
**verbose_name** | **String** | Return object's verbose_name | [readonly]
**verbose_name_plural** | **String** | Return object's plural verbose_name | [readonly]
**meta_model_name** | **String** | Return internal model name | [readonly]
**client_id** | **String** |  | 
**tenant_id** | **String** |  | 
**certificate_authorities** | Option<**Vec<uuid::Uuid>**> | Certificate authorities which issue device certificates via Intune (Cloud PKI, SCEP or PKCS profiles), used by the endpoint stage to validate certificates. This option has a higher priority than the `client_certificate` option on `Brand`. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


