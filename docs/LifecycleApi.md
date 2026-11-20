# \LifecycleApi

All URIs are relative to */api/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**lifecycle_iterations_create**](LifecycleApi.md#lifecycle_iterations_create) | **POST** /lifecycle/iterations/ | 
[**lifecycle_iterations_list_latest**](LifecycleApi.md#lifecycle_iterations_list_latest) | **GET** /lifecycle/iterations/latest/{content_type}/{object_id}/ | 
[**lifecycle_iterations_list_open**](LifecycleApi.md#lifecycle_iterations_list_open) | **GET** /lifecycle/iterations/open/ | 
[**lifecycle_reviews_create**](LifecycleApi.md#lifecycle_reviews_create) | **POST** /lifecycle/reviews/ | 
[**lifecycle_rules_create**](LifecycleApi.md#lifecycle_rules_create) | **POST** /lifecycle/rules/ | 
[**lifecycle_rules_destroy**](LifecycleApi.md#lifecycle_rules_destroy) | **DELETE** /lifecycle/rules/{id}/ | 
[**lifecycle_rules_list**](LifecycleApi.md#lifecycle_rules_list) | **GET** /lifecycle/rules/ | 
[**lifecycle_rules_partial_update**](LifecycleApi.md#lifecycle_rules_partial_update) | **PATCH** /lifecycle/rules/{id}/ | 
[**lifecycle_rules_retrieve**](LifecycleApi.md#lifecycle_rules_retrieve) | **GET** /lifecycle/rules/{id}/ | 
[**lifecycle_rules_update**](LifecycleApi.md#lifecycle_rules_update) | **PUT** /lifecycle/rules/{id}/ | 
[**lifecycle_user_expiration_rules_create**](LifecycleApi.md#lifecycle_user_expiration_rules_create) | **POST** /lifecycle/user_expiration_rules/ | 
[**lifecycle_user_expiration_rules_destroy**](LifecycleApi.md#lifecycle_user_expiration_rules_destroy) | **DELETE** /lifecycle/user_expiration_rules/{id}/ | 
[**lifecycle_user_expiration_rules_list**](LifecycleApi.md#lifecycle_user_expiration_rules_list) | **GET** /lifecycle/user_expiration_rules/ | 
[**lifecycle_user_expiration_rules_partial_update**](LifecycleApi.md#lifecycle_user_expiration_rules_partial_update) | **PATCH** /lifecycle/user_expiration_rules/{id}/ | 
[**lifecycle_user_expiration_rules_preview_create**](LifecycleApi.md#lifecycle_user_expiration_rules_preview_create) | **POST** /lifecycle/user_expiration_rules/{id}/preview/ | 
[**lifecycle_user_expiration_rules_preview_retrieve**](LifecycleApi.md#lifecycle_user_expiration_rules_preview_retrieve) | **GET** /lifecycle/user_expiration_rules/{id}/preview/ | 
[**lifecycle_user_expiration_rules_retrieve**](LifecycleApi.md#lifecycle_user_expiration_rules_retrieve) | **GET** /lifecycle/user_expiration_rules/{id}/ | 
[**lifecycle_user_expiration_rules_update**](LifecycleApi.md#lifecycle_user_expiration_rules_update) | **PUT** /lifecycle/user_expiration_rules/{id}/ | 
[**lifecycle_user_expiration_rules_used_by_list**](LifecycleApi.md#lifecycle_user_expiration_rules_used_by_list) | **GET** /lifecycle/user_expiration_rules/{id}/used_by/ | 
[**lifecycle_user_offboarding_create**](LifecycleApi.md#lifecycle_user_offboarding_create) | **POST** /lifecycle/user_offboarding/ | 
[**lifecycle_user_offboarding_destroy**](LifecycleApi.md#lifecycle_user_offboarding_destroy) | **DELETE** /lifecycle/user_offboarding/{id}/ | 
[**lifecycle_user_offboarding_list**](LifecycleApi.md#lifecycle_user_offboarding_list) | **GET** /lifecycle/user_offboarding/ | 
[**lifecycle_user_offboarding_retrieve**](LifecycleApi.md#lifecycle_user_offboarding_retrieve) | **GET** /lifecycle/user_offboarding/{id}/ | 



## lifecycle_iterations_create

> models::LifecycleIteration lifecycle_iterations_create(lifecycle_iteration_request)


Mixin to validate that a valid enterprise license exists before allowing to save the object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**lifecycle_iteration_request** | [**LifecycleIterationRequest**](LifecycleIterationRequest.md) |  | [required] |

### Return type

[**models::LifecycleIteration**](LifecycleIteration.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_iterations_list_latest

> Vec<models::LifecycleIteration> lifecycle_iterations_list_latest(content_type, object_id, ordering, search, user_is_reviewer)


Mixin to validate that a valid enterprise license exists before allowing to save the object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**content_type** | **String** |  | [required] |
**object_id** | **String** |  | [required] |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**search** | Option<**String**> | A search term. |  |
**user_is_reviewer** | Option<**bool**> |  |  |

### Return type

[**Vec<models::LifecycleIteration>**](LifecycleIteration.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_iterations_list_open

> models::PaginatedLifecycleIterationList lifecycle_iterations_list_open(ordering, page, page_size, search, user_is_reviewer)


Mixin to validate that a valid enterprise license exists before allowing to save the object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**search** | Option<**String**> | A search term. |  |
**user_is_reviewer** | Option<**bool**> |  |  |

### Return type

[**models::PaginatedLifecycleIterationList**](PaginatedLifecycleIterationList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_reviews_create

> models::Review lifecycle_reviews_create(review_request)


Mixin to validate that a valid enterprise license exists before allowing to save the object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**review_request** | [**ReviewRequest**](ReviewRequest.md) |  | [required] |

### Return type

[**models::Review**](Review.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_rules_create

> models::LifecycleRule lifecycle_rules_create(lifecycle_rule_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**lifecycle_rule_request** | [**LifecycleRuleRequest**](LifecycleRuleRequest.md) |  | [required] |

### Return type

[**models::LifecycleRule**](LifecycleRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_rules_destroy

> lifecycle_rules_destroy(id)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this lifecycle rule. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_rules_list

> models::PaginatedLifecycleRuleList lifecycle_rules_list(content_type__model, ordering, page, page_size, search)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**content_type__model** | Option<**String**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**search** | Option<**String**> | A search term. |  |

### Return type

[**models::PaginatedLifecycleRuleList**](PaginatedLifecycleRuleList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_rules_partial_update

> models::LifecycleRule lifecycle_rules_partial_update(id, patched_lifecycle_rule_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this lifecycle rule. | [required] |
**patched_lifecycle_rule_request** | Option<[**PatchedLifecycleRuleRequest**](PatchedLifecycleRuleRequest.md)> |  |  |

### Return type

[**models::LifecycleRule**](LifecycleRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_rules_retrieve

> models::LifecycleRule lifecycle_rules_retrieve(id)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this lifecycle rule. | [required] |

### Return type

[**models::LifecycleRule**](LifecycleRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_rules_update

> models::LifecycleRule lifecycle_rules_update(id, lifecycle_rule_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this lifecycle rule. | [required] |
**lifecycle_rule_request** | [**LifecycleRuleRequest**](LifecycleRuleRequest.md) |  | [required] |

### Return type

[**models::LifecycleRule**](LifecycleRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_create

> models::UserExpirationRule lifecycle_user_expiration_rules_create(user_expiration_rule_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_expiration_rule_request** | [**UserExpirationRuleRequest**](UserExpirationRuleRequest.md) |  | [required] |

### Return type

[**models::UserExpirationRule**](UserExpirationRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_destroy

> lifecycle_user_expiration_rules_destroy(id)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Expiration Rule. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_list

> models::PaginatedUserExpirationRuleList lifecycle_user_expiration_rules_list(action, enabled, group, ordering, page, page_size, pbm_uuid, search)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**action** | Option<[**OffboardingActionEnum**](OffboardingActionEnum.md)> |  |  |
**enabled** | Option<**bool**> |  |  |
**group** | Option<**uuid::Uuid**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**pbm_uuid** | Option<**uuid::Uuid**> |  |  |
**search** | Option<**String**> | A search term. |  |

### Return type

[**models::PaginatedUserExpirationRuleList**](PaginatedUserExpirationRuleList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_partial_update

> models::UserExpirationRule lifecycle_user_expiration_rules_partial_update(id, patched_user_expiration_rule_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Expiration Rule. | [required] |
**patched_user_expiration_rule_request** | Option<[**PatchedUserExpirationRuleRequest**](PatchedUserExpirationRuleRequest.md)> |  |  |

### Return type

[**models::UserExpirationRule**](UserExpirationRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_preview_create

> models::UserExpirationRulePreview lifecycle_user_expiration_rules_preview_create(id, user_expiration_rule_request)


Preview new offboardings and changes to pending rows if this rule is enabled.  POST accepts unsaved edits to the rule. Neither method saves the rule, changes offboardings, or sends warnings. Existing policy bindings still apply.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Expiration Rule. | [required] |
**user_expiration_rule_request** | [**UserExpirationRuleRequest**](UserExpirationRuleRequest.md) |  | [required] |

### Return type

[**models::UserExpirationRulePreview**](UserExpirationRulePreview.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_preview_retrieve

> models::UserExpirationRulePreview lifecycle_user_expiration_rules_preview_retrieve(id)


Preview new offboardings and changes to pending rows if this rule is enabled.  POST accepts unsaved edits to the rule. Neither method saves the rule, changes offboardings, or sends warnings. Existing policy bindings still apply.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Expiration Rule. | [required] |

### Return type

[**models::UserExpirationRulePreview**](UserExpirationRulePreview.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_retrieve

> models::UserExpirationRule lifecycle_user_expiration_rules_retrieve(id)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Expiration Rule. | [required] |

### Return type

[**models::UserExpirationRule**](UserExpirationRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_update

> models::UserExpirationRule lifecycle_user_expiration_rules_update(id, user_expiration_rule_request)


Mixin to add a used_by endpoint to return a list of all objects using this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Expiration Rule. | [required] |
**user_expiration_rule_request** | [**UserExpirationRuleRequest**](UserExpirationRuleRequest.md) |  | [required] |

### Return type

[**models::UserExpirationRule**](UserExpirationRule.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_expiration_rules_used_by_list

> Vec<models::UsedBy> lifecycle_user_expiration_rules_used_by_list(id)


Get a list of all objects that use this object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Expiration Rule. | [required] |

### Return type

[**Vec<models::UsedBy>**](UsedBy.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_offboarding_create

> models::UserOffboarding lifecycle_user_offboarding_create(user_offboarding_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_offboarding_request** | [**UserOffboardingRequest**](UserOffboardingRequest.md) |  | [required] |

### Return type

[**models::UserOffboarding**](UserOffboarding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_offboarding_destroy

> lifecycle_user_offboarding_destroy(id)


Cancel a pending offboarding instead of deleting the record.  The row is retained (as `CANCELED`) so the offboarding stays visible in the audit history; deletion would erase who scheduled and cancelled it. You cannot cancel an offboarding that targets you.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Offboarding. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_offboarding_list

> models::PaginatedUserOffboardingList lifecycle_user_offboarding_list(action, generated, ordering, page, page_size, rule, rule__isnull, search, status, user__uuid)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**action** | Option<[**OffboardingActionEnum**](OffboardingActionEnum.md)> |  |  |
**generated** | Option<**bool**> |  |  |
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**rule** | Option<**uuid::Uuid**> |  |  |
**rule__isnull** | Option<**bool**> |  |  |
**search** | Option<**String**> | A search term. |  |
**status** | Option<[**OffboardingStatusEnum**](OffboardingStatusEnum.md)> |  |  |
**user__uuid** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::PaginatedUserOffboardingList**](PaginatedUserOffboardingList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## lifecycle_user_offboarding_retrieve

> models::UserOffboarding lifecycle_user_offboarding_retrieve(id)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | A UUID string identifying this User Offboarding. | [required] |

### Return type

[**models::UserOffboarding**](UserOffboarding.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

