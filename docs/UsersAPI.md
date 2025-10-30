# \UsersAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetUsers**](UsersAPI.md#GetUsers) | **Get** /v1/users | Get the users in an organisation or scan group
[**UpdateUserPreferences**](UsersAPI.md#UpdateUserPreferences) | **Patch** /users/preferences | Update preferences for the user logged in to the current session
[**UsersApiKeyPost**](UsersAPI.md#UsersApiKeyPost) | **Post** /users/api_key | Create an API key for the user logged in to the current session



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

