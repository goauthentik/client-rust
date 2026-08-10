# \AgentsApi

All URIs are relative to */api/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**agents_agents_create**](AgentsApi.md#agents_agents_create) | **POST** /agents/agents/ | 
[**agents_agents_destroy**](AgentsApi.md#agents_agents_destroy) | **DELETE** /agents/agents/{id}/ | 
[**agents_agents_list**](AgentsApi.md#agents_agents_list) | **GET** /agents/agents/ | 
[**agents_agents_partial_update**](AgentsApi.md#agents_agents_partial_update) | **PATCH** /agents/agents/{id}/ | 
[**agents_agents_retrieve**](AgentsApi.md#agents_agents_retrieve) | **GET** /agents/agents/{id}/ | 
[**agents_agents_update**](AgentsApi.md#agents_agents_update) | **PUT** /agents/agents/{id}/ | 



## agents_agents_create

> models::AgentCreated agents_agents_create(agent_create_request)


Admin-provisioned delegate identities. An admin creates a Agent for a given parent user, then grants it access the same way as any other User -- ordinary PolicyBindings pointed at whatever it needs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**agent_create_request** | Option<[**AgentCreateRequest**](AgentCreateRequest.md)> |  |  |

### Return type

[**models::AgentCreated**](AgentCreated.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## agents_agents_destroy

> agents_agents_destroy(id)


Admin-provisioned delegate identities. An admin creates a Agent for a given parent user, then grants it access the same way as any other User -- ordinary PolicyBindings pointed at whatever it needs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | A unique integer value identifying this Agent. | [required] |

### Return type

 (empty response body)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## agents_agents_list

> models::PaginatedAgentList agents_agents_list(ordering, page, page_size, parent, search)


Admin-provisioned delegate identities. An admin creates a Agent for a given parent user, then grants it access the same way as any other User -- ordinary PolicyBindings pointed at whatever it needs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**ordering** | Option<**String**> | Which field to use when ordering the results. |  |
**page** | Option<**i32**> | A page number within the paginated result set. |  |
**page_size** | Option<**i32**> | Number of results to return per page. |  |
**parent** | Option<**i32**> |  |  |
**search** | Option<**String**> | A search term. |  |

### Return type

[**models::PaginatedAgentList**](PaginatedAgentList.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## agents_agents_partial_update

> models::Agent agents_agents_partial_update(id, patched_agent_request)


Admin-provisioned delegate identities. An admin creates a Agent for a given parent user, then grants it access the same way as any other User -- ordinary PolicyBindings pointed at whatever it needs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | A unique integer value identifying this Agent. | [required] |
**patched_agent_request** | Option<[**PatchedAgentRequest**](PatchedAgentRequest.md)> |  |  |

### Return type

[**models::Agent**](Agent.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## agents_agents_retrieve

> models::Agent agents_agents_retrieve(id)


Admin-provisioned delegate identities. An admin creates a Agent for a given parent user, then grants it access the same way as any other User -- ordinary PolicyBindings pointed at whatever it needs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | A unique integer value identifying this Agent. | [required] |

### Return type

[**models::Agent**](Agent.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## agents_agents_update

> models::Agent agents_agents_update(id, agent_request)


Admin-provisioned delegate identities. An admin creates a Agent for a given parent user, then grants it access the same way as any other User -- ordinary PolicyBindings pointed at whatever it needs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | A unique integer value identifying this Agent. | [required] |
**agent_request** | [**AgentRequest**](AgentRequest.md) |  | [required] |

### Return type

[**models::Agent**](Agent.md)

### Authorization

[authentik](../README.md#authentik)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

