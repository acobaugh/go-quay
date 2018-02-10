# \RepositorynotificationApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateRepoNotification**](RepositorynotificationApi.md#CreateRepoNotification) | **Post** /api/v1/repository/{repository}/notification/ | 
[**DeleteRepoNotification**](RepositorynotificationApi.md#DeleteRepoNotification) | **Delete** /api/v1/repository/{repository}/notification/{uuid} | 
[**GetRepoNotification**](RepositorynotificationApi.md#GetRepoNotification) | **Get** /api/v1/repository/{repository}/notification/{uuid} | 
[**ListRepoNotifications**](RepositorynotificationApi.md#ListRepoNotifications) | **Get** /api/v1/repository/{repository}/notification/ | 
[**ResetRepositoryNotificationFailures**](RepositorynotificationApi.md#ResetRepositoryNotificationFailures) | **Post** /api/v1/repository/{repository}/notification/{uuid} | 
[**TestRepoNotification**](RepositorynotificationApi.md#TestRepoNotification) | **Post** /api/v1/repository/{repository}/notification/{uuid}/test | 


# **CreateRepoNotification**
> CreateRepoNotification(ctx, repository, body)




### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**NotificationCreateRequest**](NotificationCreateRequest.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRepoNotification**
> DeleteRepoNotification(ctx, uuid, repository)


Deletes the specified notification.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **uuid** | **string**| The UUID of the notification | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepoNotification**
> GetRepoNotification(ctx, uuid, repository)


Get information for the specified notification.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **uuid** | **string**| The UUID of the notification | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListRepoNotifications**
> ListRepoNotifications(ctx, repository)


List the notifications for the specified repository.

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

# **ResetRepositoryNotificationFailures**
> ResetRepositoryNotificationFailures(ctx, uuid, repository)


Resets repository notification to 0 failures.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **uuid** | **string**| The UUID of the notification | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **TestRepoNotification**
> TestRepoNotification(ctx, uuid, repository)


Queues a test notification for this repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **uuid** | **string**| The UUID of the notification | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

