# \ScansAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddScanSeedById**](ScansAPI.md#AddScanSeedById) | **Post** /v1/scans/{id}/seeds | Add a seed to a scan by ID
[**CreateScan**](ScansAPI.md#CreateScan) | **Post** /v1/scans | Create a scan
[**DeleteScanById**](ScansAPI.md#DeleteScanById) | **Delete** /v1/scans/{id} | Delete a scan by ID
[**GetScanByID**](ScansAPI.md#GetScanByID) | **Get** /v1/scans/{id} | Get a scan by ID
[**GetScanIterationProgress**](ScansAPI.md#GetScanIterationProgress) | **Get** /v1/scans/{scan_id}/iterations/{iteration_id}/progress | Get the progress for the provided iteration
[**GetScanIterationsById**](ScansAPI.md#GetScanIterationsById) | **Get** /v1/scans/{id}/iterations | Get the Iterations for a specified scan
[**GetScanLinkTags**](ScansAPI.md#GetScanLinkTags) | **Get** /v1/scans/{id}/link_tags | Get link tags for a scan
[**GetScanSeedsById**](ScansAPI.md#GetScanSeedsById) | **Get** /v1/scans/{id}/seeds | Get the seeds for a scan by ID
[**GetScans**](ScansAPI.md#GetScans) | **Get** /v1/scans | Get the Scans for a specified scan group
[**GetScansCount**](ScansAPI.md#GetScansCount) | **Get** /v1/scans/count | Get the count of Scans for a specified scan group according to the filter settings
[**GetScreenshotById**](ScansAPI.md#GetScreenshotById) | **Get** /v1/scans/{scan_id}/screenshots/{id} | Get a web presence screenshot by ID
[**RemoveScanSeedById**](ScansAPI.md#RemoveScanSeedById) | **Delete** /v1/scans/{id}/seeds/{seed_id} | Remove a seed from a scan by ID
[**RemoveSeedTag**](ScansAPI.md#RemoveSeedTag) | **Delete** /v1/scans/{id}/seeds/{seed_id}/tags/{tag_name} | Remove a tag from a seed
[**TriggerRescanByScanId**](ScansAPI.md#TriggerRescanByScanId) | **Post** /v1/scans/{id}/rescan | Trigger rescan by scan ID
[**UpdateNodeInScanById**](ScansAPI.md#UpdateNodeInScanById) | **Patch** /v1/scans/{id}/nodes/{node_id} | Update a node by ID
[**UpdateScanById**](ScansAPI.md#UpdateScanById) | **Patch** /v1/scans/{id} | Update a scan by ID



## AddScanSeedById

> NodeResponse AddScanSeedById(ctx, id).CreateScanSeedRequest(createScanSeedRequest).Execute()

Add a seed to a scan by ID



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
	id := "id_example" // string | Scan ID
	createScanSeedRequest := *asm.NewCreateScanSeedRequest("Name_example", "Type_example") // CreateScanSeedRequest | Parameters to create the new seed

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.AddScanSeedById(context.Background(), id).CreateScanSeedRequest(createScanSeedRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.AddScanSeedById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddScanSeedById`: NodeResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.AddScanSeedById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddScanSeedByIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createScanSeedRequest** | [**CreateScanSeedRequest**](CreateScanSeedRequest.md) | Parameters to create the new seed | 

### Return type

[**NodeResponse**](NodeResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateScan

> ScanResponse CreateScan(ctx).CreateScanRequest(createScanRequest).Execute()

Create a scan



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
	createScanRequest := *asm.NewCreateScanRequest("Name_example", "ScanGroupId_example", asm.ScanType("adhoc")) // CreateScanRequest | Parameters to create the new scan

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.CreateScan(context.Background()).CreateScanRequest(createScanRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.CreateScan``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateScan`: ScanResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.CreateScan`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateScanRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createScanRequest** | [**CreateScanRequest**](CreateScanRequest.md) | Parameters to create the new scan | 

### Return type

[**ScanResponse**](ScanResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteScanById

> DeleteScanById(ctx, id).Execute()

Delete a scan by ID



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
	id := "id_example" // string | Scan ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.ScansAPI.DeleteScanById(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.DeleteScanById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteScanByIdRequest struct via the builder pattern


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


## GetScanByID

> ScanResponse GetScanByID(ctx, id).Expand(expand).Execute()

Get a scan by ID



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
	id := "id_example" // string | Scan ID
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScanByID(context.Background(), id).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScanByID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanByID`: ScanResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScanByID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanByIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**ScanResponse**](ScanResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanIterationProgress

> ScanProgressResponse GetScanIterationProgress(ctx, scanId, iterationId).Execute()

Get the progress for the provided iteration



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
	scanId := "scanId_example" // string | Scan ID
	iterationId := "iterationId_example" // string | Iteration ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScanIterationProgress(context.Background(), scanId, iterationId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScanIterationProgress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanIterationProgress`: ScanProgressResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScanIterationProgress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 
**iterationId** | **string** | Iteration ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanIterationProgressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ScanProgressResponse**](ScanProgressResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanIterationsById

> []ScanIterationResponse GetScanIterationsById(ctx, id).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()

Get the Iterations for a specified scan



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
	id := "id_example" // string | Scan ID
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScanIterationsById(context.Background(), id).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScanIterationsById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanIterationsById`: []ScanIterationResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScanIterationsById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanIterationsByIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 

### Return type

[**[]ScanIterationResponse**](ScanIterationResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanLinkTags

> []ScanLinkTagResponse GetScanLinkTags(ctx, id).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Execute()

Get link tags for a scan



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
	id := "id_example" // string | Scan ID
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScanLinkTags(context.Background(), id).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScanLinkTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanLinkTags`: []ScanLinkTagResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScanLinkTags`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanLinkTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**[]ScanLinkTagResponse**](ScanLinkTagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanSeedsById

> []SeedsResponseInner GetScanSeedsById(ctx, id).Expand(expand).Execute()

Get the seeds for a scan by ID

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
	id := "id_example" // string | Scan ID
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScanSeedsById(context.Background(), id).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScanSeedsById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanSeedsById`: []SeedsResponseInner
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScanSeedsById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanSeedsByIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**[]SeedsResponseInner**](SeedsResponseInner.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScans

> []ScanResponse GetScans(ctx).ScanGroupId(scanGroupId).Type_(type_).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Search(search).SearchSeeds(searchSeeds).IncludeDisabled(includeDisabled).IncludeDeleted(includeDeleted).Execute()

Get the Scans for a specified scan group



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
	scanGroupId := "scanGroupId_example" // string | Scan Group ID
	type_ := []string{"Type_example"} // []string | Filter by scan types
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)
	search := "search_example" // string | Search string (optional)
	searchSeeds := true // bool | Include seeds in text search (optional)
	includeDisabled := true // bool | Include disabled scans (optional)
	includeDeleted := true // bool | Include deleted scans (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScans(context.Background()).ScanGroupId(scanGroupId).Type_(type_).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Search(search).SearchSeeds(searchSeeds).IncludeDisabled(includeDisabled).IncludeDeleted(includeDeleted).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScans``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScans`: []ScanResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScans`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetScansRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scanGroupId** | **string** | Scan Group ID | 
 **type_** | **[]string** | Filter by scan types | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **expand** | **[]string** | Fields to expand with additional information | 
 **search** | **string** | Search string | 
 **searchSeeds** | **bool** | Include seeds in text search | 
 **includeDisabled** | **bool** | Include disabled scans | 
 **includeDeleted** | **bool** | Include deleted scans | 

### Return type

[**[]ScanResponse**](ScanResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScansCount

> InlineObject GetScansCount(ctx).ScanGroupId(scanGroupId).Type_(type_).Search(search).SearchSeeds(searchSeeds).IncludeDisabled(includeDisabled).IncludeDeleted(includeDeleted).Execute()

Get the count of Scans for a specified scan group according to the filter settings



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
	scanGroupId := "scanGroupId_example" // string | Scan Group ID
	type_ := []string{"Type_example"} // []string | Filter by scan types
	search := "search_example" // string | Search string (optional)
	searchSeeds := true // bool | Include seeds in text search (optional)
	includeDisabled := true // bool | Include disabled scans (optional)
	includeDeleted := true // bool | Include deleted scans (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScansCount(context.Background()).ScanGroupId(scanGroupId).Type_(type_).Search(search).SearchSeeds(searchSeeds).IncludeDisabled(includeDisabled).IncludeDeleted(includeDeleted).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScansCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScansCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScansCount`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetScansCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scanGroupId** | **string** | Scan Group ID | 
 **type_** | **[]string** | Filter by scan types | 
 **search** | **string** | Search string | 
 **searchSeeds** | **bool** | Include seeds in text search | 
 **includeDisabled** | **bool** | Include disabled scans | 
 **includeDeleted** | **bool** | Include deleted scans | 

### Return type

[**InlineObject**](InlineObject.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScreenshotById

> *os.File GetScreenshotById(ctx, id, scanId).Execute()

Get a web presence screenshot by ID



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
	id := "id_example" // string | Screenshot ID
	scanId := "scanId_example" // string | Scan ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.GetScreenshotById(context.Background(), id, scanId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.GetScreenshotById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScreenshotById`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.GetScreenshotById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Screenshot ID | 
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScreenshotByIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[***os.File**](*os.File.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: image/webp, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveScanSeedById

> RemoveScanSeedById(ctx, id, seedId).Execute()

Remove a seed from a scan by ID



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
	id := "id_example" // string | Scan ID
	seedId := "seedId_example" // string | Seed ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.ScansAPI.RemoveScanSeedById(context.Background(), id, seedId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.RemoveScanSeedById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 
**seedId** | **string** | Seed ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveScanSeedByIdRequest struct via the builder pattern


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


## RemoveSeedTag

> RemoveSeedTag(ctx, id, seedId, tagName).Execute()

Remove a tag from a seed



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
	id := "id_example" // string | Scan ID
	seedId := "seedId_example" // string | Seed ID
	tagName := "tagName_example" // string | Tag name to remove from the seed

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.ScansAPI.RemoveSeedTag(context.Background(), id, seedId, tagName).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.RemoveSeedTag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 
**seedId** | **string** | Seed ID | 
**tagName** | **string** | Tag name to remove from the seed | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveSeedTagRequest struct via the builder pattern


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


## TriggerRescanByScanId

> TriggerRescanByScanId(ctx, id).Execute()

Trigger rescan by scan ID



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
	id := "id_example" // string | Scan ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.ScansAPI.TriggerRescanByScanId(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.TriggerRescanByScanId``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiTriggerRescanByScanIdRequest struct via the builder pattern


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


## UpdateNodeInScanById

> GenericGraphNode UpdateNodeInScanById(ctx, id, nodeId).UpdateNodeRequest(updateNodeRequest).Execute()

Update a node by ID



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
	id := "id_example" // string | Scan ID
	nodeId := "nodeId_example" // string | Node ID
	updateNodeRequest := *asm.NewUpdateNodeRequest() // UpdateNodeRequest | Parameters to update the node

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.UpdateNodeInScanById(context.Background(), id, nodeId).UpdateNodeRequest(updateNodeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.UpdateNodeInScanById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateNodeInScanById`: GenericGraphNode
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.UpdateNodeInScanById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 
**nodeId** | **string** | Node ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateNodeInScanByIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateNodeRequest** | [**UpdateNodeRequest**](UpdateNodeRequest.md) | Parameters to update the node | 

### Return type

[**GenericGraphNode**](GenericGraphNode.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateScanById

> ScanResponse UpdateScanById(ctx, id).UpdateScanByIdRequest(updateScanByIdRequest).Execute()

Update a scan by ID



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
	id := "id_example" // string | Scan ID
	updateScanByIdRequest := *asm.NewUpdateScanByIdRequest() // UpdateScanByIdRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScansAPI.UpdateScanById(context.Background(), id).UpdateScanByIdRequest(updateScanByIdRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScansAPI.UpdateScanById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateScanById`: ScanResponse
	fmt.Fprintf(os.Stdout, "Response from `ScansAPI.UpdateScanById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateScanByIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateScanByIdRequest** | [**UpdateScanByIdRequest**](UpdateScanByIdRequest.md) |  | 

### Return type

[**ScanResponse**](ScanResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

