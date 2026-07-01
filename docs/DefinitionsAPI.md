# \DefinitionsAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetDefinition**](DefinitionsAPI.md#GetDefinition) | **Get** /v1/definitions/definition | Get Definition



## GetDefinition

> GetDefinition200Response GetDefinition(ctx).Lang(lang).Key(key).Subkey(subkey).Execute()

Get Definition



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
	lang := "lang_example" // string | Language code (e.g. en_gb)
	key := "key_example" // string | Definition key (e.g. urn:issue:mail:policy:missing)
	subkey := "subkey_example" // string | Definition subkey (e.g. description)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.DefinitionsAPI.GetDefinition(context.Background()).Lang(lang).Key(key).Subkey(subkey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefinitionsAPI.GetDefinition``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDefinition`: GetDefinition200Response
	fmt.Fprintf(os.Stdout, "Response from `DefinitionsAPI.GetDefinition`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetDefinitionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lang** | **string** | Language code (e.g. en_gb) | 
 **key** | **string** | Definition key (e.g. urn:issue:mail:policy:missing) | 
 **subkey** | **string** | Definition subkey (e.g. description) | 

### Return type

[**GetDefinition200Response**](GetDefinition200Response.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

