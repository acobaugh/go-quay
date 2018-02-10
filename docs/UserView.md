# UserView

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Organizations** | [**[]interface{}**](interface{}.md) | Information about the organizations in which the user is a member | [optional] [default to null]
**Verified** | **bool** | Whether the user&#39;s email address has been verified | [optional] [default to null]
**Avatar** | [***interface{}**](interface{}.md) | Avatar data representing the user&#39;s icon | [default to null]
**Anonymous** | **bool** | true if this user data represents a guest user | [default to null]
**Logins** | [**[]interface{}**](interface{}.md) | The list of external login providers against which the user has authenticated | [optional] [default to null]
**CanCreateRepo** | **bool** | Whether the user has permission to create repositories | [optional] [default to null]
**PreferredNamespace** | **bool** | If true, the user&#39;s namespace is the preferred namespace to display | [optional] [default to null]
**Email** | **string** | The user&#39;s email address | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


