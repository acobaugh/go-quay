# \TeamApi

All URIs are relative to *https://quay.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteOrganizationTeam**](TeamApi.md#DeleteOrganizationTeam) | **Delete** /api/v1/organization/{orgname}/team/{teamname} | 
[**DeleteOrganizationTeamMember**](TeamApi.md#DeleteOrganizationTeamMember) | **Delete** /api/v1/organization/{orgname}/team/{teamname}/members/{membername} | 
[**DeleteTeamMemberEmailInvite**](TeamApi.md#DeleteTeamMemberEmailInvite) | **Delete** /api/v1/organization/{orgname}/team/{teamname}/invite/{email} | 
[**GetOrganizationTeamMembers**](TeamApi.md#GetOrganizationTeamMembers) | **Get** /api/v1/organization/{orgname}/team/{teamname}/members | 
[**GetOrganizationTeamPermissions**](TeamApi.md#GetOrganizationTeamPermissions) | **Get** /api/v1/organization/{orgname}/team/{teamname}/permissions | 
[**InviteTeamMemberEmail**](TeamApi.md#InviteTeamMemberEmail) | **Put** /api/v1/organization/{orgname}/team/{teamname}/invite/{email} | 
[**UpdateOrganizationTeam**](TeamApi.md#UpdateOrganizationTeam) | **Put** /api/v1/organization/{orgname}/team/{teamname} | 
[**UpdateOrganizationTeamMember**](TeamApi.md#UpdateOrganizationTeamMember) | **Put** /api/v1/organization/{orgname}/team/{teamname}/members/{membername} | 


# **DeleteOrganizationTeam**
> DeleteOrganizationTeam(ctx, orgname, teamname)


Delete the specified team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **teamname** | **string**| The name of the team | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteOrganizationTeamMember**
> DeleteOrganizationTeamMember(ctx, orgname, membername, teamname)


Delete a member of a team. If the user is merely invited to join         the team, then the invite is removed instead.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **membername** | **string**| The username of the team member | 
  **teamname** | **string**| The name of the team | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteTeamMemberEmailInvite**
> DeleteTeamMemberEmailInvite(ctx, orgname, email, teamname)


Delete an invite of an email address to join a team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**|  | 
  **email** | **string**|  | 
  **teamname** | **string**|  | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganizationTeamMembers**
> GetOrganizationTeamMembers(ctx, orgname, teamname, optional)


Retrieve the list of members for the specified team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **teamname** | **string**| The name of the team | 
 **optional** | **map[string]interface{}** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a map[string]interface{}.

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgname** | **string**| The name of the organization | 
 **teamname** | **string**| The name of the team | 
 **includePending** | **bool**| Whether to include pending members | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetOrganizationTeamPermissions**
> GetOrganizationTeamPermissions(ctx, orgname, teamname)


Returns the list of repository permissions for the org's team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **teamname** | **string**| The name of the team | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **InviteTeamMemberEmail**
> InviteTeamMemberEmail(ctx, orgname, email, teamname)


Invites an email address to an existing team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**|  | 
  **email** | **string**|  | 
  **teamname** | **string**|  | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateOrganizationTeam**
> UpdateOrganizationTeam(ctx, orgname, teamname, body)


Update the org-wide permission for the specified team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **teamname** | **string**| The name of the team | 
  **body** | [**TeamDescription**](TeamDescription.md)| Request body contents. | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateOrganizationTeamMember**
> UpdateOrganizationTeamMember(ctx, orgname, membername, teamname)


Adds or invites a member to an existing team.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for logging, tracing, authentication, etc.
  **orgname** | **string**| The name of the organization | 
  **membername** | **string**| The username of the team member | 
  **teamname** | **string**| The name of the team | 

### Return type

 (empty response body)

### Authorization

[oauth2_implicit](../README.md#oauth2_implicit)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

