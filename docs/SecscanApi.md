# \SecscanApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetRepoImageSecurity**](SecscanApi.md#GetRepoImageSecurity) | **Get** /api/v1/repository/{repository}/image/{imageid}/security | 
[**GetRepoManifestSecurity**](SecscanApi.md#GetRepoManifestSecurity) | **Get** /api/v1/repository/{repository}/manifest/{manifestref}/security | 


# **GetRepoImageSecurity**
> GetRepoImageSecurity(ctx, repository, imageid, optional)


Fetches the features and vulnerabilities (if any) for a repository image.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **imageid** | **string**| The image ID | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **imageid** | **string**| The image ID | 
 **vulnerabilities** | **bool**| Include vulnerabilities informations | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepoManifestSecurity**
> GetRepoManifestSecurity(ctx, manifestref, repository, optional)




### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **manifestref** | **string**| The digest of the manifest | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **manifestref** | **string**| The digest of the manifest | 
 **repository** | **string**| The full path of the repository. e.g. namespace/name | 
 **vulnerabilities** | **bool**| Include vulnerabilities informations | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

