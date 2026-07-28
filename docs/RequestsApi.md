# \RequestsApi

All URIs are relative to */api/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**requests_grant_requests_create**](RequestsApi.md#requests_grant_requests_create) | **POST** /requests/grant-requests/ | 
[**requests_grant_requests_destroy**](RequestsApi.md#requests_grant_requests_destroy) | **DELETE** /requests/grant-requests/{uuid}/ | 
[**requests_grant_requests_fulfill_partial_update**](RequestsApi.md#requests_grant_requests_fulfill_partial_update) | **PATCH** /requests/grant-requests/{uuid}/fulfill/ | 
[**requests_grant_requests_list**](RequestsApi.md#requests_grant_requests_list) | **GET** /requests/grant-requests/ | 
[**requests_grant_requests_pending_review_list**](RequestsApi.md#requests_grant_requests_pending_review_list) | **GET** /requests/grant-requests/pending_review/ | 
[**requests_grant_requests_retrieve**](RequestsApi.md#requests_grant_requests_retrieve) | **GET** /requests/grant-requests/{uuid}/ | 
[**requests_grant_requests_revoke_destroy**](RequestsApi.md#requests_grant_requests_revoke_destroy) | **DELETE** /requests/grant-requests/{uuid}/revoke/ | 
[**requests_rule_bindings_create**](RequestsApi.md#requests_rule_bindings_create) | **POST** /requests/rule-bindings/ | 
[**requests_rule_bindings_destroy**](RequestsApi.md#requests_rule_bindings_destroy) | **DELETE** /requests/rule-bindings/{uuid}/ | 
[**requests_rule_bindings_list**](RequestsApi.md#requests_rule_bindings_list) | **GET** /requests/rule-bindings/ | 
[**requests_rule_bindings_partial_update**](RequestsApi.md#requests_rule_bindings_partial_update) | **PATCH** /requests/rule-bindings/{uuid}/ | 
[**requests_rule_bindings_retrieve**](RequestsApi.md#requests_rule_bindings_retrieve) | **GET** /requests/rule-bindings/{uuid}/ | 
[**requests_rule_bindings_update**](RequestsApi.md#requests_rule_bindings_update) | **PUT** /requests/rule-bindings/{uuid}/ | 
[**requests_rule_bindings_used_by_list**](RequestsApi.md#requests_rule_bindings_used_by_list) | **GET** /requests/rule-bindings/{uuid}/used_by/ | 
[**requests_rule_child_bindings_create**](RequestsApi.md#requests_rule_child_bindings_create) | **POST** /requests/rule-child-bindings/ | 
[**requests_rule_child_bindings_destroy**](RequestsApi.md#requests_rule_child_bindings_destroy) | **DELETE** /requests/rule-child-bindings/{uuid}/ | 
[**requests_rule_child_bindings_list**](RequestsApi.md#requests_rule_child_bindings_list) | **GET** /requests/rule-child-bindings/ | 
[**requests_rule_child_bindings_partial_update**](RequestsApi.md#requests_rule_child_bindings_partial_update) | **PATCH** /requests/rule-child-bindings/{uuid}/ | 
[**requests_rule_child_bindings_retrieve**](RequestsApi.md#requests_rule_child_bindings_retrieve) | **GET** /requests/rule-child-bindings/{uuid}/ | 
[**requests_rule_child_bindings_update**](RequestsApi.md#requests_rule_child_bindings_update) | **PUT** /requests/rule-child-bindings/{uuid}/ | 
[**requests_rule_child_bindings_used_by_list**](RequestsApi.md#requests_rule_child_bindings_used_by_list) | **GET** /requests/rule-child-bindings/{uuid}/used_by/ | 
[**requests_rules_create**](RequestsApi.md#requests_rules_create) | **POST** /requests/rules/ | 
[**requests_rules_destroy**](RequestsApi.md#requests_rules_destroy) | **DELETE** /requests/rules/{uuid}/ | 
[**requests_rules_list**](RequestsApi.md#requests_rules_list) | **GET** /requests/rules/ | 
[**requests_rules_partial_update**](RequestsApi.md#requests_rules_partial_update) | **PATCH** /requests/rules/{uuid}/ | 
[**requests_rules_retrieve**](RequestsApi.md#requests_rules_retrieve) | **GET** /requests/rules/{uuid}/ | 
[**requests_rules_update**](RequestsApi.md#requests_rules_update) | **PUT** /requests/rules/{uuid}/ | 
[**requests_rules_used_by_list**](RequestsApi.md#requests_rules_used_by_list) | **GET** /requests/rules/{uuid}/used_by/ | 



## requests_grant_requests_create

> models::Link requests_grant_requests_create(grant_request_create_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**grant_request_create_request** | [**GrantRequestCreateRequest**](GrantRequestCreateRequest.md) |  | [required] |

### Return type

[**models::Link**](Link.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_grant_requests_destroy

> requests_grant_requests_destroy(uuid)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Grant Request. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_grant_requests_fulfill_partial_update

> requests_grant_requests_fulfill_partial_update(uuid, patched_grant_request_fulfill_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Grant Request. | [required] |
**patched_grant_request_fulfill_request** | Option<[**PatchedGrantRequestFulfillRequest**](PatchedGrantRequestFulfillRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_grant_requests_list

> models::PaginatedGrantRequestList requests_grant_requests_list(created_by, ordering, page, page_size, search, status)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**created_by** | Option<**i32**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**search** | Option<**String**> | A search term. |  |
**status** | Option<[**RequestStatus**](RequestStatus.md)> |  |  |

### Return type

[**models::PaginatedGrantRequestList**](PaginatedGrantRequestList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_grant_requests_pending_review_list

> models::PaginatedGrantRequestList requests_grant_requests_pending_review_list(created_by, ordering, page, page_size, search, status)


List pending grant requests the current user is eligible to review.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**created_by** | Option<**i32**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**search** | Option<**String**> | A search term. |  |
**status** | Option<[**RequestStatus**](RequestStatus.md)> |  |  |

### Return type

[**models::PaginatedGrantRequestList**](PaginatedGrantRequestList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_grant_requests_retrieve

> models::GrantRequest requests_grant_requests_retrieve(uuid)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Grant Request. | [required] |

### Return type

[**models::GrantRequest**](GrantRequest.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_grant_requests_revoke_destroy

> requests_grant_requests_revoke_destroy(uuid)


Immediately end an active grant. Available to the same reviewers who could approve it in the first place.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Grant Request. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_bindings_create

> models::RequestRuleBinding requests_rule_bindings_create(request_rule_binding_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**request_rule_binding_request** | [**RequestRuleBindingRequest**](RequestRuleBindingRequest.md) |  | [required] |

### Return type

[**models::RequestRuleBinding**](RequestRuleBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_bindings_destroy

> requests_rule_bindings_destroy(uuid)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Binding. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_bindings_list

> models::PaginatedRequestRuleBindingList requests_rule_bindings_list(ordering, page, page_size, rule, search, target)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**rule** | Option<**uuid::Uuid**> |  |  |
**search** | Option<**String**> | A search term. |  |
**target** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::PaginatedRequestRuleBindingList**](PaginatedRequestRuleBindingList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_bindings_partial_update

> models::RequestRuleBinding requests_rule_bindings_partial_update(uuid, patched_request_rule_binding_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Binding. | [required] |
**patched_request_rule_binding_request** | Option<[**PatchedRequestRuleBindingRequest**](PatchedRequestRuleBindingRequest.md)> |  |  |

### Return type

[**models::RequestRuleBinding**](RequestRuleBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_bindings_retrieve

> models::RequestRuleBinding requests_rule_bindings_retrieve(uuid)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Binding. | [required] |

### Return type

[**models::RequestRuleBinding**](RequestRuleBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_bindings_update

> models::RequestRuleBinding requests_rule_bindings_update(uuid, request_rule_binding_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Binding. | [required] |
**request_rule_binding_request** | [**RequestRuleBindingRequest**](RequestRuleBindingRequest.md) |  | [required] |

### Return type

[**models::RequestRuleBinding**](RequestRuleBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_bindings_used_by_list

> Vec<models::UsedBy> requests_rule_bindings_used_by_list(uuid)


Get a list of all objects that use this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Binding. | [required] |

### Return type

[**Vec<models::UsedBy>**](UsedBy.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_child_bindings_create

> models::RequestRuleChildBinding requests_rule_child_bindings_create(request_rule_child_binding_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**request_rule_child_binding_request** | [**RequestRuleChildBindingRequest**](RequestRuleChildBindingRequest.md) |  | [required] |

### Return type

[**models::RequestRuleChildBinding**](RequestRuleChildBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_child_bindings_destroy

> requests_rule_child_bindings_destroy(uuid)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Child Binding. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_child_bindings_list

> models::PaginatedRequestRuleChildBindingList requests_rule_child_bindings_list(binding, ordering, page, page_size, search, target)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**binding** | Option<**uuid::Uuid**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**search** | Option<**String**> | A search term. |  |
**target** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::PaginatedRequestRuleChildBindingList**](PaginatedRequestRuleChildBindingList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_child_bindings_partial_update

> models::RequestRuleChildBinding requests_rule_child_bindings_partial_update(uuid, patched_request_rule_child_binding_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Child Binding. | [required] |
**patched_request_rule_child_binding_request** | Option<[**PatchedRequestRuleChildBindingRequest**](PatchedRequestRuleChildBindingRequest.md)> |  |  |

### Return type

[**models::RequestRuleChildBinding**](RequestRuleChildBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_child_bindings_retrieve

> models::RequestRuleChildBinding requests_rule_child_bindings_retrieve(uuid)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Child Binding. | [required] |

### Return type

[**models::RequestRuleChildBinding**](RequestRuleChildBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_child_bindings_update

> models::RequestRuleChildBinding requests_rule_child_bindings_update(uuid, request_rule_child_binding_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Child Binding. | [required] |
**request_rule_child_binding_request** | [**RequestRuleChildBindingRequest**](RequestRuleChildBindingRequest.md) |  | [required] |

### Return type

[**models::RequestRuleChildBinding**](RequestRuleChildBinding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rule_child_bindings_used_by_list

> Vec<models::UsedBy> requests_rule_child_bindings_used_by_list(uuid)


Get a list of all objects that use this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule Child Binding. | [required] |

### Return type

[**Vec<models::UsedBy>**](UsedBy.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rules_create

> models::RequestRule requests_rules_create(request_rule_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**request_rule_request** | [**RequestRuleRequest**](RequestRuleRequest.md) |  | [required] |

### Return type

[**models::RequestRule**](RequestRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rules_destroy

> requests_rules_destroy(uuid)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rules_list

> models::PaginatedRequestRuleList requests_rules_list(name, ordering, page, page_size, pbm_uuid, request_flow__slug, search)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**pbm_uuid** | Option<**uuid::Uuid**> |  |  |
**request_flow__slug** | Option<**String**> |  |  |
**search** | Option<**String**> | A search term. |  |

### Return type

[**models::PaginatedRequestRuleList**](PaginatedRequestRuleList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rules_partial_update

> models::RequestRule requests_rules_partial_update(uuid, patched_request_rule_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule. | [required] |
**patched_request_rule_request** | Option<[**PatchedRequestRuleRequest**](PatchedRequestRuleRequest.md)> |  |  |

### Return type

[**models::RequestRule**](RequestRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rules_retrieve

> models::RequestRule requests_rules_retrieve(uuid)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule. | [required] |

### Return type

[**models::RequestRule**](RequestRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rules_update

> models::RequestRule requests_rules_update(uuid, request_rule_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule. | [required] |
**request_rule_request** | [**RequestRuleRequest**](RequestRuleRequest.md) |  | [required] |

### Return type

[**models::RequestRule**](RequestRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## requests_rules_used_by_list

> Vec<models::UsedBy> requests_rules_used_by_list(uuid)


Get a list of all objects that use this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **uuid::Uuid** | A UUID string identifying this Request Rule. | [required] |

### Return type

[**Vec<models::UsedBy>**](UsedBy.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

