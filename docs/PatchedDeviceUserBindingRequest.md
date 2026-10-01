# PatchedDeviceUserBindingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**policy** | Option<**uuid::Uuid**> |  | [optional]
**group** | Option<**uuid::Uuid**> |  | [optional]
**user** | Option<**i32**> |  | [optional]
**target** | Option<**uuid::Uuid**> |  | [optional]
**negate** | Option<**bool**> | Negates the outcome of the policy. Messages are unaffected. | [optional]
**enabled** | Option<**bool**> |  | [optional]
**dry_run** | Option<**bool**> | Execute the policy but ignore its result. | [optional]
**order** | Option<**i32**> |  | [optional]
**timeout** | Option<**u32**> | Timeout after which Policy execution is terminated. | [optional]
**failure_result** | Option<**bool**> | Result if the Policy execution fails. | [optional]
**is_primary** | Option<**bool**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


