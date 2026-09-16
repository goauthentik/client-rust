# \DebugApi

All URIs are relative to */api/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**debug_log_create**](DebugApi.md#debug_log_create) | **POST** /debug/log/ | 



## debug_log_create

> debug_log_create(server_log_request)


Debug-only endpoint to allow frontend to log messages, usable when browser develooper-tools aren't available.  Never available in production.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**server_log_request** | [**ServerLogRequest**](ServerLogRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

