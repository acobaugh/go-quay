# \PermissionApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ChangeTeamPermissions**](PermissionApi.md#ChangeTeamPermissions) | **Put** /api/v1/repository/{repository}/permissions/team/{teamname} | 
[**ChangeUserPermissions**](PermissionApi.md#ChangeUserPermissions) | **Put** /api/v1/repository/{repository}/permissions/user/{username} | 
[**DeleteTeamPermissions**](PermissionApi.md#DeleteTeamPermissions) | **Delete** /api/v1/repository/{repository}/permissions/team/{teamname} | 
[**DeleteUserPermissions**](PermissionApi.md#DeleteUserPermissions) | **Delete** /api/v1/repository/{repository}/permissions/user/{username} | 
[**GetTeamPermissions**](PermissionApi.md#GetTeamPermissions) | **Get** /api/v1/repository/{repository}/permissions/team/{teamname} | 
[**GetUserPermissions**](PermissionApi.md#GetUserPermissions) | **Get** /api/v1/repository/{repository}/permissions/user/{username} | 
[**GetUserTransitivePermission**](PermissionApi.md#GetUserTransitivePermission) | **Get** /api/v1/repository/{repository}/permissions/user/{username}/transitive | 
[**ListRepoTeamPermissions**](PermissionApi.md#ListRepoTeamPermissions) | **Get** /api/v1/repository/{repository}/permissions/team/ | 
[**ListRepoUserPermissions**](PermissionApi.md#ListRepoUserPermissions) | **Get** /api/v1/repository/{repository}/permissions/user/ | 


# **ChangeTeamPermissions**
> ChangeTeamPermissions(ctx, teamname, repository, body)


Update the existing team permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **teamname** | **string**| The name of the team to which the permission applies | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**TeamPermission**](TeamPermission.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ChangeUserPermissions**
> ChangeUserPermissions(ctx, username, repository, body)


Update the perimssions for an existing repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **username** | **string**| The username of the user to which the permission applies | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 
  **body** | [**UserPermission**](UserPermission.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteTeamPermissions**
> DeleteTeamPermissions(ctx, teamname, repository)


Delete the permission for the specified team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **teamname** | **string**| The name of the team to which the permission applies | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteUserPermissions**
> DeleteUserPermissions(ctx, username, repository)


Delete the permission for the user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **username** | **string**| The username of the user to which the permission applies | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetTeamPermissions**
> GetTeamPermissions(ctx, teamname, repository)


Fetch the permission for the specified team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **teamname** | **string**| The name of the team to which the permission applies | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUserPermissions**
> GetUserPermissions(ctx, username, repository)


Get the permission for the specified user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **username** | **string**| The username of the user to which the permission applies | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUserTransitivePermission**
> GetUserTransitivePermission(ctx, username, repository)


Get the fetch the permission for the specified user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **username** | **string**| The username of the user to which the permissions apply | 
  **repository** | **string**| The full path of the repository. e.g. namespace/name | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListRepoTeamPermissions**
> ListRepoTeamPermissions(ctx, repository)


List all team permission.

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

# **ListRepoUserPermissions**
> ListRepoUserPermissions(ctx, repository)


List all user permissions.

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

