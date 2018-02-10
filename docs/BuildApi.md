# \BuildApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelRepoBuild**](BuildApi.md#CancelRepoBuild) | **Delete** /api/v1/repository/{repository}/build/{build_uuid} | 
[**GetRepoBuild**](BuildApi.md#GetRepoBuild) | **Get** /api/v1/repository/{repository}/build/{build_uuid} | 
[**GetRepoBuildLogs**](BuildApi.md#GetRepoBuildLogs) | **Get** /api/v1/repository/{repository}/build/{build_uuid}/logs | 
[**GetRepoBuildStatus**](BuildApi.md#GetRepoBuildStatus) | **Get** /api/v1/repository/{repository}/build/{build_uuid}/status | 
[**GetRepoBuilds**](BuildApi.md#GetRepoBuilds) | **Get** /api/v1/repository/{repository}/build/ | 
[**RequestRepoBuild**](BuildApi.md#RequestRepoBuild) | **Post** /api/v1/repository/{repository}/build/ | 


# **CancelRepoBuild**
> CancelRepoBuild(ctx, buildUuid, repository)


Cancels a repository build.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **buildUuid** | **string**| The UUID of the build | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepoBuild**
> GetRepoBuild(ctx, buildUuid, repository)


Returns information about a build.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **buildUuid** | **string**| The UUID of the build | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepoBuildLogs**
> GetRepoBuildLogs(ctx, buildUuid, repository)


Return the build logs for the build specified by the build uuid.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **buildUuid** | **string**| The UUID of the build | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepoBuildStatus**
> GetRepoBuildStatus(ctx, buildUuid, repository)


Return the status for the builds specified by the build uuids.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **buildUuid** | **string**| The UUID of the build | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepoBuilds**
> GetRepoBuilds(ctx, repository, optional)


Get the list of repository builds.

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
 **since** | **int32**| Returns all builds since the given unix timecode | 
 **limit** | **int32**| The maximum number of builds to return | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RequestRepoBuild**
> RequestRepoBuild(ctx, repository, body)


Request that a repository be built and pushed from the specified input.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**RepositoryBuildRequest**](RepositoryBuildRequest.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

