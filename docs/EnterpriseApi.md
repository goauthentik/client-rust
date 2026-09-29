# \EnterpriseApi

All URIs are relative to */api/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**enterprise_license_create**](EnterpriseApi.md#enterprise_license_create) | **POST** /enterprise/license/ | 
[**enterprise_license_destroy**](EnterpriseApi.md#enterprise_license_destroy) | **DELETE** /enterprise/license/{license_uuid}/ | 
[**enterprise_license_install_id_retrieve**](EnterpriseApi.md#enterprise_license_install_id_retrieve) | **GET** /enterprise/license/install_id/ | 
[**enterprise_license_list**](EnterpriseApi.md#enterprise_license_list) | **GET** /enterprise/license/ | 
[**enterprise_license_partial_update**](EnterpriseApi.md#enterprise_license_partial_update) | **PATCH** /enterprise/license/{license_uuid}/ | 
[**enterprise_license_retrieve**](EnterpriseApi.md#enterprise_license_retrieve) | **GET** /enterprise/license/{license_uuid}/ | 
[**enterprise_license_summary_retrieve**](EnterpriseApi.md#enterprise_license_summary_retrieve) | **GET** /enterprise/license/summary/ | 
[**enterprise_license_update**](EnterpriseApi.md#enterprise_license_update) | **PUT** /enterprise/license/{license_uuid}/ | 
[**enterprise_license_used_by_list**](EnterpriseApi.md#enterprise_license_used_by_list) | **GET** /enterprise/license/{license_uuid}/used_by/ | 
[**enterprise_license_user_counts_retrieve**](EnterpriseApi.md#enterprise_license_user_counts_retrieve) | **GET** /enterprise/license/user_counts/ | 



## enterprise_license_create

> models::License enterprise_license_create(license_request)


License Viewset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**license_request** | [**LicenseRequest**](LicenseRequest.md) |  | [required] |

### Return type

[**models::License**](License.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_destroy

> enterprise_license_destroy(license_uuid)


License Viewset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**license_uuid** | **uuid::Uuid** | A UUID string identifying this License. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_install_id_retrieve

> models::InstallId enterprise_license_install_id_retrieve()


Get install_id

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::InstallId**](InstallID.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_list

> models::PaginatedLicenseList enterprise_license_list(name, ordering, page, page_size, search)


License Viewset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**search** | Option<**String**> | A search term. |  |

### Return type

[**models::PaginatedLicenseList**](PaginatedLicenseList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_partial_update

> models::License enterprise_license_partial_update(license_uuid, patched_license_request)


License Viewset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**license_uuid** | **uuid::Uuid** | A UUID string identifying this License. | [required] |
**patched_license_request** | Option<[**PatchedLicenseRequest**](PatchedLicenseRequest.md)> |  |  |

### Return type

[**models::License**](License.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_retrieve

> models::License enterprise_license_retrieve(license_uuid)


License Viewset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**license_uuid** | **uuid::Uuid** | A UUID string identifying this License. | [required] |

### Return type

[**models::License**](License.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_summary_retrieve

> models::LicenseSummary enterprise_license_summary_retrieve(cached)


Get the total license status

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cached** | Option<**bool**> |  |  |[default to true]

### Return type

[**models::LicenseSummary**](LicenseSummary.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_update

> models::License enterprise_license_update(license_uuid, license_request)


License Viewset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**license_uuid** | **uuid::Uuid** | A UUID string identifying this License. | [required] |
**license_request** | [**LicenseRequest**](LicenseRequest.md) |  | [required] |

### Return type

[**models::License**](License.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_used_by_list

> Vec<models::UsedBy> enterprise_license_used_by_list(license_uuid)


Get a list of all objects that use this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**license_uuid** | **uuid::Uuid** | A UUID string identifying this License. | [required] |

### Return type

[**Vec<models::UsedBy>**](UsedBy.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## enterprise_license_user_counts_retrieve

> models::LicenseUserCounts enterprise_license_user_counts_retrieve(count_steps, end, start)


Get active user totals and counts for relative or absolute date ranges.  At least one positive relative count step or a complete absolute range is required. Relative and absolute ranges may be combined. Range starts are inclusive and ends are exclusive. Counts include currently active, non-anonymous accounts.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**count_steps** | Option<[**Vec<String>**](String.md)> | Positive relative periods, such as 'days=30' or 'weeks=3;days=2'. |  |
**end** | Option<**chrono::DateTime<chrono::FixedOffset>**> | Exclusive end of an absolute range; must be provided with start. |  |
**start** | Option<**chrono::DateTime<chrono::FixedOffset>**> | Inclusive start of an absolute range; must be provided with end. |  |

### Return type

[**models::LicenseUserCounts**](LicenseUserCounts.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

