# \PrototypeApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateOrganizationPrototypePermission**](PrototypeApi.md#CreateOrganizationPrototypePermission) | **Post** /api/v1/organization/{orgname}/prototypes | 
[**DeleteOrganizationPrototypePermission**](PrototypeApi.md#DeleteOrganizationPrototypePermission) | **Delete** /api/v1/organization/{orgname}/prototypes/{prototypeid} | 
[**GetOrganizationPrototypePermissions**](PrototypeApi.md#GetOrganizationPrototypePermissions) | **Get** /api/v1/organization/{orgname}/prototypes | 
[**UpdateOrganizationPrototypePermission**](PrototypeApi.md#UpdateOrganizationPrototypePermission) | **Put** /api/v1/organization/{orgname}/prototypes/{prototypeid} | 


# **CreateOrganizationPrototypePermission**
> CreateOrganizationPrototypePermission(ctx, orgname, body)


Create a new permission prototype.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **body** | [**NewPrototype**](NewPrototype.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteOrganizationPrototypePermission**
> DeleteOrganizationPrototypePermission(ctx, orgname, prototypeid)


Delete an existing permission prototype.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **prototypeid** | **string**| The ID of the prototype | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganizationPrototypePermissions**
> GetOrganizationPrototypePermissions(ctx, orgname)


List the existing prototypes for this organization.

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

# **UpdateOrganizationPrototypePermission**
> UpdateOrganizationPrototypePermission(ctx, orgname, prototypeid, body)


Update the role of an existing permission prototype.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **prototypeid** | **string**| The ID of the prototype | 
  **body** | [**PrototypeUpdate**](PrototypeUpdate.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

