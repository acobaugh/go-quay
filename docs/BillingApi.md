# \BillingApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListOrgInvoices**](BillingApi.md#ListOrgInvoices) | **Get** /api/v1/organization/{orgname}/invoices | 
[**ListPlans**](BillingApi.md#ListPlans) | **Get** /api/v1/plans/ | 


# **ListOrgInvoices**
> ListOrgInvoices(ctx, orgname)


List the invoices for the specified orgnaization.

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

# **ListPlans**
> ListPlans(ctx, )


List the avaialble plans.

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

