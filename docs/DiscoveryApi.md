# \DiscoveryApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Discovery**](DiscoveryApi.md#Discovery) | **Get** /api/v1/discovery | 


# **Discovery**
> Discovery(ctx, optional)


List all of the API endpoints available in the swagger API format.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **internal** | **bool**| Whether to include internal APIs. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

