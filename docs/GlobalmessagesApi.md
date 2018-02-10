# \GlobalmessagesApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateGlobalMessage**](GlobalmessagesApi.md#CreateGlobalMessage) | **Post** /api/v1/messages | 
[**GetGlobalMessages**](GlobalmessagesApi.md#GetGlobalMessages) | **Get** /api/v1/messages | 


# **CreateGlobalMessage**
> CreateGlobalMessage(ctx, body)


Create a message

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **body** | [**CreateMessage**](CreateMessage.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetGlobalMessages**
> GetGlobalMessages(ctx, )


Return a super users messages

### Required Parameters
This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

