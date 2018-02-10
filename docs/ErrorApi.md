# \ErrorApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetErrorDescription**](ErrorApi.md#GetErrorDescription) | **Get** /api/v1/error/{error_type} | 


# **GetErrorDescription**
> ApiErrorDescription GetErrorDescription(ctx, errorType)


Get a detailed description of the error

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **errorType** | **string**| The error code identifying the type of error. | 

### Return type

[**ApiErrorDescription**](ApiErrorDescription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

