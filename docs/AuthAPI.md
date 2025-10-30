# \AuthAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetState**](AuthAPI.md#GetState) | **Get** /auth | Get the auth state and associated user for the request



## GetState

> AuthResponse GetState(ctx).Execute()

Get the auth state and associated user for the request

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
	resp, r, err := apiClient.AuthAPI.GetState(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.GetState``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetState`: AuthResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.GetState`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetStateRequest struct via the builder pattern


### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

