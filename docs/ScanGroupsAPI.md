# \ScanGroupsAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateScanGroup**](ScanGroupsAPI.md#CreateScanGroup) | **Post** /v1/scan_groups | Create a new scan group
[**DeleteScanGroupByID**](ScanGroupsAPI.md#DeleteScanGroupByID) | **Delete** /v1/scan_groups/{id} | Delete a scan group by ID
[**GetScanGroupByID**](ScanGroupsAPI.md#GetScanGroupByID) | **Get** /v1/scan_groups/{id} | Get a scan group by ID
[**GetScanGroups**](ScanGroupsAPI.md#GetScanGroups) | **Get** /v1/scan_groups | Get the Scan Groups for a specified organisation
[**UpdateScanGroupByID**](ScanGroupsAPI.md#UpdateScanGroupByID) | **Patch** /v1/scan_groups/{id} | Update a scan group by ID



## CreateScanGroup

> ScanGroupResponse CreateScanGroup(ctx).ScanGroupCreateRequestBody(scanGroupCreateRequestBody).Execute()

Create a new scan group



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
	scanGroupCreateRequestBody := *asm.NewScanGroupCreateRequestBody("Name_example", "OrganisationId_example") // ScanGroupCreateRequestBody | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanGroupsAPI.CreateScanGroup(context.Background()).ScanGroupCreateRequestBody(scanGroupCreateRequestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanGroupsAPI.CreateScanGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateScanGroup`: ScanGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanGroupsAPI.CreateScanGroup`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateScanGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scanGroupCreateRequestBody** | [**ScanGroupCreateRequestBody**](ScanGroupCreateRequestBody.md) |  | 

### Return type

[**ScanGroupResponse**](ScanGroupResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteScanGroupByID

> DeleteScanGroupByID(ctx, id).Execute()

Delete a scan group by ID



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
	id := "id_example" // string | Scan Group ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.ScanGroupsAPI.DeleteScanGroupByID(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanGroupsAPI.DeleteScanGroupByID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan Group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteScanGroupByIDRequest struct via the builder pattern


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


## GetScanGroupByID

> ScanGroupResponse GetScanGroupByID(ctx, id).Expand(expand).Execute()

Get a scan group by ID



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
	id := "id_example" // string | Scan Group ID
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanGroupsAPI.GetScanGroupByID(context.Background(), id).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanGroupsAPI.GetScanGroupByID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanGroupByID`: ScanGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanGroupsAPI.GetScanGroupByID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan Group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanGroupByIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**ScanGroupResponse**](ScanGroupResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanGroups

> []ScanGroupResponse GetScanGroups(ctx).OrganisationId(organisationId).Limit(limit).Offset(offset).Order(order).Dir(dir).IncludeDeleted(includeDeleted).Expand(expand).Execute()

Get the Scan Groups for a specified organisation



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
	organisationId := "organisationId_example" // string | Organisation ID
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	includeDeleted := true // bool | Included deleted entries in results (optional)
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanGroupsAPI.GetScanGroups(context.Background()).OrganisationId(organisationId).Limit(limit).Offset(offset).Order(order).Dir(dir).IncludeDeleted(includeDeleted).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanGroupsAPI.GetScanGroups``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanGroups`: []ScanGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanGroupsAPI.GetScanGroups`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetScanGroupsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisationId** | **string** | Organisation ID | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **includeDeleted** | **bool** | Included deleted entries in results | 
 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**[]ScanGroupResponse**](ScanGroupResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateScanGroupByID

> ScanGroupResponse UpdateScanGroupByID(ctx, id).ScanGroupUpdateRequestBody(scanGroupUpdateRequestBody).Execute()

Update a scan group by ID



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
	id := "id_example" // string | Scan Group ID
	scanGroupUpdateRequestBody := *asm.NewScanGroupUpdateRequestBody() // ScanGroupUpdateRequestBody | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanGroupsAPI.UpdateScanGroupByID(context.Background(), id).ScanGroupUpdateRequestBody(scanGroupUpdateRequestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanGroupsAPI.UpdateScanGroupByID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateScanGroupByID`: ScanGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanGroupsAPI.UpdateScanGroupByID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan Group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateScanGroupByIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **scanGroupUpdateRequestBody** | [**ScanGroupUpdateRequestBody**](ScanGroupUpdateRequestBody.md) |  | 

### Return type

[**ScanGroupResponse**](ScanGroupResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

