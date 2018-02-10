# \TagApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ChangeTag**](TagApi.md#ChangeTag) | **Put** /api/v1/repository/{repository}/tag/{tag} | 
[**DeleteFullTag**](TagApi.md#DeleteFullTag) | **Delete** /api/v1/repository/{repository}/tag/{tag} | 
[**ListRepoTags**](TagApi.md#ListRepoTags) | **Get** /api/v1/repository/{repository}/tag/ | 
[**ListTagImages**](TagApi.md#ListTagImages) | **Get** /api/v1/repository/{repository}/tag/{tag}/images | 
[**RestoreTag**](TagApi.md#RestoreTag) | **Post** /api/v1/repository/{repository}/tag/{tag}/restore | 


# **ChangeTag**
> ChangeTag(ctx, tag, repository, body)


Change which image a tag points to or create a new tag.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **tag** | **string**| The name of the tag | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**ChangeTag**](ChangeTag.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteFullTag**
> DeleteFullTag(ctx, tag, repository)


Delete the specified repository tag.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **tag** | **string**| The name of the tag | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListRepoTags**
> ListRepoTags(ctx, repository, optional)




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
 **page** | **int32**| Page index for the results. Default 1. | 
 **limit** | **int32**| Limit to the number of results to return per page. Max 100. | 
 **specificTag** | **string**| Filters the tags to the specific tag. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListTagImages**
> ListTagImages(ctx, tag, repository, optional)


List the images for the specified repository tag.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **tag** | **string**| The name of the tag | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tag** | **string**| The name of the tag | 
 **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **owned** | **bool**| If specified, only images wholely owned by this tag are returned. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RestoreTag**
> RestoreTag(ctx, tag, repository, body)


Restores a repository tag back to a previous image in the repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **tag** | **string**| The name of the tag | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**RestoreTag**](RestoreTag.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

