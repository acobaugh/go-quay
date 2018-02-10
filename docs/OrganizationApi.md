# \OrganizationApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ChangeOrganizationDetails**](OrganizationApi.md#ChangeOrganizationDetails) | **Put** /api/v1/organization/{orgname} | 
[**CreateOrganization**](OrganizationApi.md#CreateOrganization) | **Post** /api/v1/organization/ | 
[**CreateOrganizationApplication**](OrganizationApi.md#CreateOrganizationApplication) | **Post** /api/v1/organization/{orgname}/applications | 
[**DeleteAdminedOrganization**](OrganizationApi.md#DeleteAdminedOrganization) | **Delete** /api/v1/organization/{orgname} | 
[**DeleteOrganizationApplication**](OrganizationApi.md#DeleteOrganizationApplication) | **Delete** /api/v1/organization/{orgname}/applications/{client_id} | 
[**GetApplicationInformation**](OrganizationApi.md#GetApplicationInformation) | **Get** /api/v1/app/{client_id} | 
[**GetOrganization**](OrganizationApi.md#GetOrganization) | **Get** /api/v1/organization/{orgname} | 
[**GetOrganizationApplication**](OrganizationApi.md#GetOrganizationApplication) | **Get** /api/v1/organization/{orgname}/applications/{client_id} | 
[**GetOrganizationApplications**](OrganizationApi.md#GetOrganizationApplications) | **Get** /api/v1/organization/{orgname}/applications | 
[**GetOrganizationMember**](OrganizationApi.md#GetOrganizationMember) | **Get** /api/v1/organization/{orgname}/members/{membername} | 
[**GetOrganizationMembers**](OrganizationApi.md#GetOrganizationMembers) | **Get** /api/v1/organization/{orgname}/members | 
[**RemoveOrganizationMember**](OrganizationApi.md#RemoveOrganizationMember) | **Delete** /api/v1/organization/{orgname}/members/{membername} | 
[**UpdateOrganizationApplication**](OrganizationApi.md#UpdateOrganizationApplication) | **Put** /api/v1/organization/{orgname}/applications/{client_id} | 


# **ChangeOrganizationDetails**
> ChangeOrganizationDetails(ctx, orgname, body)


Change the details for the specified organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **body** | [**UpdateOrg**](UpdateOrg.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateOrganization**
> CreateOrganization(ctx, body)


Create a new organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **body** | [**NewOrg**](NewOrg.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateOrganizationApplication**
> CreateOrganizationApplication(ctx, orgname, body)


Creates a new application under this organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **body** | [**NewApp**](NewApp.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAdminedOrganization**
> DeleteAdminedOrganization(ctx, orgname)


Deletes the specified organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteOrganizationApplication**
> DeleteOrganizationApplication(ctx, orgname, clientId)


Deletes the application under this organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **clientId** | **string**| The OAuth client ID | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetApplicationInformation**
> GetApplicationInformation(ctx, clientId)


Get information on the specified application.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **clientId** | **string**| The OAuth client ID | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganization**
> GetOrganization(ctx, orgname)


Get the details for the specified organization

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganizationApplication**
> GetOrganizationApplication(ctx, orgname, clientId)


Retrieves the application with the specified client_id under the specified organization

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **clientId** | **string**| The OAuth client ID | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganizationApplications**
> GetOrganizationApplications(ctx, orgname)


List the applications for the specified organization

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganizationMember**
> GetOrganizationMember(ctx, orgname, membername)


Retrieves the details of a member of the organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **membername** | **string**| The username of the organization member | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganizationMembers**
> GetOrganizationMembers(ctx, orgname)


List the human members of the specified organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RemoveOrganizationMember**
> RemoveOrganizationMember(ctx, orgname, membername)


Removes a member from an organization, revoking all its repository         priviledges and removing it from all teams in the organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **membername** | **string**| The username of the organization member | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateOrganizationApplication**
> UpdateOrganizationApplication(ctx, orgname, clientId, body)


Updates an application under this organization.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **clientId** | **string**| The OAuth client ID | 
  **body** | [**UpdateApp**](UpdateApp.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

