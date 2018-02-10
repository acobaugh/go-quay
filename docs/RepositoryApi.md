# \RepositoryApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ChangeRepoTrust**](RepositoryApi.md#ChangeRepoTrust) | **Post** /api/v1/repository/{repository}/changetrust | 
[**ChangeRepoVisibility**](RepositoryApi.md#ChangeRepoVisibility) | **Post** /api/v1/repository/{repository}/changevisibility | 
[**CreateRepo**](RepositoryApi.md#CreateRepo) | **Post** /api/v1/repository | 
[**DeleteRepository**](RepositoryApi.md#DeleteRepository) | **Delete** /api/v1/repository/{repository} | 
[**GetRepo**](RepositoryApi.md#GetRepo) | **Get** /api/v1/repository/{repository} | 
[**ListRepos**](RepositoryApi.md#ListRepos) | **Get** /api/v1/repository | 
[**UpdateRepo**](RepositoryApi.md#UpdateRepo) | **Put** /api/v1/repository/{repository} | 


# **ChangeRepoTrust**
> ChangeRepoTrust(ctx, repository, body)


Change the visibility of a repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**ChangeRepoTrust**](ChangeRepoTrust.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ChangeRepoVisibility**
> ChangeRepoVisibility(ctx, repository, body)


Change the visibility of a repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**ChangeVisibility**](ChangeVisibility.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRepo**
> CreateRepo(ctx, body)


Create a new repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **body** | [**NewRepo**](NewRepo.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRepository**
> DeleteRepository(ctx, repository)


Delete a repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepo**
> GetRepo(ctx, repository, optional)


Fetch the specified repository.

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
 **includeStats** | **bool**| Whether to include action statistics | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListRepos**
> ListRepos(ctx, optional)


Fetch the list of repositories visible to the current user under a variety of situations.

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
 **repoKind** | **string**| The kind of repositories to return | 
 **popularity** | **bool**| Whether to include the repository&#39;s popularity metric. | 
 **lastModified** | **bool**| Whether to include when the repository was last modified. | 
 **public** | **bool**| Adds any repositories visible to the user by virtue of being public | 
 **starred** | **bool**| Filters the repositories returned to those starred by the user | 
 **namespace** | **string**| Filters the repositories returned to this namespace | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateRepo**
> UpdateRepo(ctx, repository, body)


Update the description in the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**RepoUpdate**](RepoUpdate.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

