# \OrganisationsAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteOrganisationAsset**](OrganisationsAPI.md#DeleteOrganisationAsset) | **Delete** /v1/orgs/{id}/asset/{key} | Delete an organisation asset
[**GetOrganisationAsset**](OrganisationsAPI.md#GetOrganisationAsset) | **Get** /v1/orgs/{id}/asset/{key} | Get an organisation asset by key
[**GetOrganisationByID**](OrganisationsAPI.md#GetOrganisationByID) | **Get** /v1/orgs/{id} | Get an organisation by ID
[**GetOrganisations**](OrganisationsAPI.md#GetOrganisations) | **Get** /v1/orgs | Get the organisations for which the current user is a member



## DeleteOrganisationAsset

> DeleteOrganisationAsset(ctx, id, key).Execute()

Delete an organisation asset



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
	id := "id_example" // string | Organisation ID
	key := "key_example" // string | Asset key

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.OrganisationsAPI.DeleteOrganisationAsset(context.Background(), id, key).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganisationsAPI.DeleteOrganisationAsset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Organisation ID | 
**key** | **string** | Asset key | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteOrganisationAssetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOrganisationAsset

> OrganisationAssetResponse GetOrganisationAsset(ctx, id, key).Execute()

Get an organisation asset by key



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
	id := "id_example" // string | Organisation ID
	key := "key_example" // string | Asset key

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganisationsAPI.GetOrganisationAsset(context.Background(), id, key).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganisationsAPI.GetOrganisationAsset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOrganisationAsset`: OrganisationAssetResponse
	fmt.Fprintf(os.Stdout, "Response from `OrganisationsAPI.GetOrganisationAsset`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Organisation ID | 
**key** | **string** | Asset key | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetOrganisationAssetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**OrganisationAssetResponse**](OrganisationAssetResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOrganisationByID

> OrganisationResponse GetOrganisationByID(ctx, id).Expand(expand).Execute()

Get an organisation by ID



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
	id := "id_example" // string | Organisation ID
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganisationsAPI.GetOrganisationByID(context.Background(), id).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganisationsAPI.GetOrganisationByID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOrganisationByID`: OrganisationResponse
	fmt.Fprintf(os.Stdout, "Response from `OrganisationsAPI.GetOrganisationByID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetOrganisationByIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**OrganisationResponse**](OrganisationResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOrganisations

> []OrganisationResponse GetOrganisations(ctx).Limit(limit).Offset(offset).Order(order).Dir(dir).IncludeDeleted(includeDeleted).Expand(expand).Execute()

Get the organisations for which the current user is a member



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
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	includeDeleted := true // bool | Included deleted entries in results (optional)
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganisationsAPI.GetOrganisations(context.Background()).Limit(limit).Offset(offset).Order(order).Dir(dir).IncludeDeleted(includeDeleted).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganisationsAPI.GetOrganisations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOrganisations`: []OrganisationResponse
	fmt.Fprintf(os.Stdout, "Response from `OrganisationsAPI.GetOrganisations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetOrganisationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **includeDeleted** | **bool** | Included deleted entries in results | 
 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**[]OrganisationResponse**](OrganisationResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

