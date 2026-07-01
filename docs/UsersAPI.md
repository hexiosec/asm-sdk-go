# \UsersAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CountUserAPIKeys**](UsersAPI.md#CountUserAPIKeys) | **Get** /users/api_key/count | Get API key count for the user logged in to the current session
[**GetUsers**](UsersAPI.md#GetUsers) | **Get** /v1/users | Get the users in an organisation or scan group
[**ListUserAPIKeys**](UsersAPI.md#ListUserAPIKeys) | **Get** /users/api_key | Get API keys for the user logged in to the current session
[**RevokeUserAPIKey**](UsersAPI.md#RevokeUserAPIKey) | **Delete** /users/api_key/{key_id} | Revoke an API key for the user logged in to the current session
[**UpdateUserPreferences**](UsersAPI.md#UpdateUserPreferences) | **Patch** /users/preferences | Update preferences for the user logged in to the current session
[**UsersApiKeyPost**](UsersAPI.md#UsersApiKeyPost) | **Post** /users/api_key | Create an API key for the user logged in to the current session



## CountUserAPIKeys

> InlineObject CountUserAPIKeys(ctx).Execute()

Get API key count for the user logged in to the current session

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.CountUserAPIKeys(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.CountUserAPIKeys``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CountUserAPIKeys`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.CountUserAPIKeys`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiCountUserAPIKeysRequest struct via the builder pattern


### Return type

[**InlineObject**](InlineObject.md)

### Authorization

[SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUsers

> []UserResponse GetUsers(ctx).OrganisationId(organisationId).ScanGroupId(scanGroupId).Execute()

Get the users in an organisation or scan group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {
	organisationId := "organisationId_example" // string | Organisation ID (optional)
	scanGroupId := "scanGroupId_example" // string | Scan Group ID (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.GetUsers(context.Background()).OrganisationId(organisationId).ScanGroupId(scanGroupId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.GetUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUsers`: []UserResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.GetUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisationId** | **string** | Organisation ID | 
 **scanGroupId** | **string** | Scan Group ID | 

### Return type

[**[]UserResponse**](UserResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListUserAPIKeys

> []UsersAPIKeyResponse ListUserAPIKeys(ctx).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()

Get API keys for the user logged in to the current session

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 10)
	offset := int32(56) // int32 |  (optional) (default to 0)
	order := "order_example" // string |  (optional) (default to "created")
	dir := "dir_example" // string |  (optional) (default to "desc")

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.ListUserAPIKeys(context.Background()).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.ListUserAPIKeys``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListUserAPIKeys`: []UsersAPIKeyResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.ListUserAPIKeys`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListUserAPIKeysRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 10]
 **offset** | **int32** |  | [default to 0]
 **order** | **string** |  | [default to &quot;created&quot;]
 **dir** | **string** |  | [default to &quot;desc&quot;]

### Return type

[**[]UsersAPIKeyResponse**](UsersAPIKeyResponse.md)

### Authorization

[SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevokeUserAPIKey

> RevokeUserAPIKey(ctx, keyId).XCSRFToken(xCSRFToken).Execute()

Revoke an API key for the user logged in to the current session

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {
	keyId := "keyId_example" // string | 
	xCSRFToken := "xCSRFToken_example" // string | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.UsersAPI.RevokeUserAPIKey(context.Background(), keyId).XCSRFToken(xCSRFToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.RevokeUserAPIKey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**keyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevokeUserAPIKeyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xCSRFToken** | **string** |  | 

### Return type

 (empty response body)

### Authorization

[SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateUserPreferences

> UserRowResponse UpdateUserPreferences(ctx).UpdateUserPreferencesRequest(updateUserPreferencesRequest).Execute()

Update preferences for the user logged in to the current session

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {
	updateUserPreferencesRequest := *asm.NewUpdateUserPreferencesRequest() // UpdateUserPreferencesRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UpdateUserPreferences(context.Background()).UpdateUserPreferencesRequest(updateUserPreferencesRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UpdateUserPreferences``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateUserPreferences`: UserRowResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UpdateUserPreferences`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUpdateUserPreferencesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **updateUserPreferencesRequest** | [**UpdateUserPreferencesRequest**](UpdateUserPreferencesRequest.md) |  | 

### Return type

[**UserRowResponse**](UserRowResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersApiKeyPost

> UsersCreateAPIKeyResponse UsersApiKeyPost(ctx).XCSRFToken(xCSRFToken).UsersCreateAPIKeyRequest(usersCreateAPIKeyRequest).Execute()

Create an API key for the user logged in to the current session

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {
	xCSRFToken := "xCSRFToken_example" // string | API Keys can only be created when logged in via session authentication, which requires the session CSRF token to be set. 
	usersCreateAPIKeyRequest := *asm.NewUsersCreateAPIKeyRequest("Test API key", "168h") // UsersCreateAPIKeyRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersApiKeyPost(context.Background()).XCSRFToken(xCSRFToken).UsersCreateAPIKeyRequest(usersCreateAPIKeyRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersApiKeyPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersApiKeyPost`: UsersCreateAPIKeyResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersApiKeyPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsersApiKeyPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xCSRFToken** | **string** | API Keys can only be created when logged in via session authentication, which requires the session CSRF token to be set.  | 
 **usersCreateAPIKeyRequest** | [**UsersCreateAPIKeyRequest**](UsersCreateAPIKeyRequest.md) |  | 

### Return type

[**UsersCreateAPIKeyResponse**](UsersCreateAPIKeyResponse.md)

### Authorization

[SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

