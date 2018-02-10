# \LogsApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetAggregateOrgLogs**](LogsApi.md#GetAggregateOrgLogs) | **Get** /api/v1/organization/{orgname}/aggregatelogs | 
[**GetAggregateRepoLogs**](LogsApi.md#GetAggregateRepoLogs) | **Get** /api/v1/repository/{repository}/aggregatelogs | 
[**GetAggregateUserLogs**](LogsApi.md#GetAggregateUserLogs) | **Get** /api/v1/user/aggregatelogs | 
[**ListOrgLogs**](LogsApi.md#ListOrgLogs) | **Get** /api/v1/organization/{orgname}/logs | 
[**ListRepoLogs**](LogsApi.md#ListRepoLogs) | **Get** /api/v1/repository/{repository}/logs | 
[**ListUserLogs**](LogsApi.md#ListUserLogs) | **Get** /api/v1/user/logs | 


# **GetAggregateOrgLogs**
> GetAggregateOrgLogs(ctx, orgname, optional)


Gets the aggregated logs for the specified organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgname** | **string**| The name of the organization | 
 **performer** | **string**| Username for which to filter logs. | 
 **endtime** | **string**| Latest time to which to get logs. (%m/%d/%Y %Z) | 
 **starttime** | **string**| Earliest time from which to get logs. (%m/%d/%Y %Z) | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAggregateRepoLogs**
> GetAggregateRepoLogs(ctx, repository, optional)


Returns the aggregated logs for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **endtime** | **string**| Latest time to which to get logs (%m/%d/%Y %Z) | 
 **starttime** | **string**| Earliest time from which to get logs (%m/%d/%Y %Z) | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAggregateUserLogs**
> GetAggregateUserLogs(ctx, optional)


Returns the aggregated logs for the current user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **performer** | **string**| Username for which to filter logs. | 
 **endtime** | **string**| Latest time to which to get logs. (%m/%d/%Y %Z) | 
 **starttime** | **string**| Earliest time from which to get logs. (%m/%d/%Y %Z) | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListOrgLogs**
> ListOrgLogs(ctx, orgname, optional)


List the logs for the specified organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgname** | **string**| The name of the organization | 
 **nextPage** | **string**| The page token for the next page | 
 **page** | **int32**| The page number for the logs | 
 **performer** | **string**| Username for which to filter logs. | 
 **endtime** | **string**| Latest time to which to get logs. (%m/%d/%Y %Z) | 
 **starttime** | **string**| Earliest time from which to get logs. (%m/%d/%Y %Z) | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListRepoLogs**
> ListRepoLogs(ctx, repository, optional)


List the logs for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **nextPage** | **string**| The page token for the next page | 
 **page** | **int32**| The page number for the logs | 
 **endtime** | **string**| Latest time to which to get logs (%m/%d/%Y %Z) | 
 **starttime** | **string**| Earliest time from which to get logs (%m/%d/%Y %Z) | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListUserLogs**
> ListUserLogs(ctx, optional)


List the logs for the current user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nextPage** | **string**| The page token for the next page | 
 **performer** | **string**| Username for which to filter logs. | 
 **endtime** | **string**| Latest time to which to get logs. (%m/%d/%Y %Z) | 
 **starttime** | **string**| Earliest time from which to get logs. (%m/%d/%Y %Z) | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

