# \TagsAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddTagToNode**](TagsAPI.md#AddTagToNode) | **Post** /v1/tags/nodes/{node_id} | Add a tag to a node
[**AddTagToScan**](TagsAPI.md#AddTagToScan) | **Post** /v1/tags/scans/{scan_id} | Add a tag to a scan
[**AddTagToSupplierScan**](TagsAPI.md#AddTagToSupplierScan) | **Post** /v1/tags/supplier_scans/{supplier_scan_group_id} | Add a tag to a supplier scan group
[**CreateTagByOrganisationID**](TagsAPI.md#CreateTagByOrganisationID) | **Post** /v1/tags/organisation/{org_id} | Create a tag for an organisation
[**DeleteTagByOrganisationID**](TagsAPI.md#DeleteTagByOrganisationID) | **Delete** /v1/tags/organisation/{org_id}/{tag_id} | Delete a tag for an organisation
[**GetScanTagsByScanID**](TagsAPI.md#GetScanTagsByScanID) | **Get** /v1/tags/scans/{scan_id} | Get tags for a scan
[**GetSupplierScanTagsBySupplierScanGroupID**](TagsAPI.md#GetSupplierScanTagsBySupplierScanGroupID) | **Get** /v1/tags/supplier_scans/{supplier_scan_group_id} | Get tags for a supplier scan group
[**GetTagsByOrganisationID**](TagsAPI.md#GetTagsByOrganisationID) | **Get** /v1/tags/organisation/{org_id} | Get tags for an organisation
[**GetTagsByOrganisationIDCount**](TagsAPI.md#GetTagsByOrganisationIDCount) | **Get** /v1/tags/organisation/{org_id}/count | Get tag count for an organisation
[**RemoveTagFromLink**](TagsAPI.md#RemoveTagFromLink) | **Delete** /v1/tags/links/{link_id}/{tag_id} | Remove a tag from a link
[**RemoveTagFromNode**](TagsAPI.md#RemoveTagFromNode) | **Delete** /v1/tags/nodes/{node_id}/{tag_id} | Remove a tag from a node
[**RemoveTagFromScan**](TagsAPI.md#RemoveTagFromScan) | **Delete** /v1/tags/scans/{scan_id}/{tag_id} | Remove a tag from a scan
[**RemoveTagFromSupplierScan**](TagsAPI.md#RemoveTagFromSupplierScan) | **Delete** /v1/tags/supplier_scans/{supplier_scan_group_id}/{tag_id} | Remove a tag from a supplier scan group
[**TagExistsByOrganisationID**](TagsAPI.md#TagExistsByOrganisationID) | **Get** /v1/tags/organisation/{org_id}/exists | Check whether a tag exists for an organisation
[**UpdateTagByOrganisationID**](TagsAPI.md#UpdateTagByOrganisationID) | **Put** /v1/tags/organisation/{org_id}/{tag_id} | Update a tag for an organisation



## AddTagToNode

> NodeTagResponse AddTagToNode(ctx, nodeId).AddTagToNodeRequest(addTagToNodeRequest).Execute()

Add a tag to a node



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
	nodeId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Node ID
	addTagToNodeRequest := *asm.NewAddTagToNodeRequest("TagId_example") // AddTagToNodeRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.AddTagToNode(context.Background(), nodeId).AddTagToNodeRequest(addTagToNodeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.AddTagToNode``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddTagToNode`: NodeTagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.AddTagToNode`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**nodeId** | **string** | Node ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddTagToNodeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **addTagToNodeRequest** | [**AddTagToNodeRequest**](AddTagToNodeRequest.md) |  | 

### Return type

[**NodeTagResponse**](NodeTagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AddTagToScan

> ScanTagResponse AddTagToScan(ctx, scanId).AddTagToScanRequest(addTagToScanRequest).Execute()

Add a tag to a scan



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
	scanId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Scan ID
	addTagToScanRequest := *asm.NewAddTagToScanRequest("TagName_example") // AddTagToScanRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.AddTagToScan(context.Background(), scanId).AddTagToScanRequest(addTagToScanRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.AddTagToScan``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddTagToScan`: ScanTagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.AddTagToScan`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddTagToScanRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **addTagToScanRequest** | [**AddTagToScanRequest**](AddTagToScanRequest.md) |  | 

### Return type

[**ScanTagResponse**](ScanTagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AddTagToSupplierScan

> SupplierScanTagResponse AddTagToSupplierScan(ctx, supplierScanGroupId).AddTagToSupplierScanRequest(addTagToSupplierScanRequest).Execute()

Add a tag to a supplier scan group



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
	supplierScanGroupId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Supplier Scan Group ID
	addTagToSupplierScanRequest := *asm.NewAddTagToSupplierScanRequest("ScanId_example") // AddTagToSupplierScanRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.AddTagToSupplierScan(context.Background(), supplierScanGroupId).AddTagToSupplierScanRequest(addTagToSupplierScanRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.AddTagToSupplierScan``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddTagToSupplierScan`: SupplierScanTagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.AddTagToSupplierScan`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**supplierScanGroupId** | **string** | Supplier Scan Group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddTagToSupplierScanRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **addTagToSupplierScanRequest** | [**AddTagToSupplierScanRequest**](AddTagToSupplierScanRequest.md) |  | 

### Return type

[**SupplierScanTagResponse**](SupplierScanTagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateTagByOrganisationID

> TagResponse CreateTagByOrganisationID(ctx, orgId).CreateTagByOrganisationIDRequest(createTagByOrganisationIDRequest).Execute()

Create a tag for an organisation



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
	orgId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Organisation ID
	createTagByOrganisationIDRequest := *asm.NewCreateTagByOrganisationIDRequest("Name_example") // CreateTagByOrganisationIDRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.CreateTagByOrganisationID(context.Background(), orgId).CreateTagByOrganisationIDRequest(createTagByOrganisationIDRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.CreateTagByOrganisationID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTagByOrganisationID`: TagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.CreateTagByOrganisationID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateTagByOrganisationIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createTagByOrganisationIDRequest** | [**CreateTagByOrganisationIDRequest**](CreateTagByOrganisationIDRequest.md) |  | 

### Return type

[**TagResponse**](TagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTagByOrganisationID

> DeleteTagByOrganisationID(ctx, orgId, tagId).Execute()

Delete a tag for an organisation



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
	orgId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Organisation ID
	tagId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Tag ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.TagsAPI.DeleteTagByOrganisationID(context.Background(), orgId, tagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.DeleteTagByOrganisationID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 
**tagId** | **string** | Tag ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTagByOrganisationIDRequest struct via the builder pattern


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


## GetScanTagsByScanID

> []ScanTagResponse GetScanTagsByScanID(ctx, scanId).UpdatedSince(updatedSince).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Execute()

Get tags for a scan



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {
	scanId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Scan ID
	updatedSince := time.Now() // time.Time | Only return scan tags updated at or after this timestamp (optional)
	limit := int32(56) // int32 | Maximum number of entries to return (optional)
	offset := int32(56) // int32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.GetScanTagsByScanID(context.Background(), scanId).UpdatedSince(updatedSince).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.GetScanTagsByScanID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanTagsByScanID`: []ScanTagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.GetScanTagsByScanID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanTagsByScanIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updatedSince** | **time.Time** | Only return scan tags updated at or after this timestamp | 
 **limit** | **int32** | Maximum number of entries to return | 
 **offset** | **int32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**[]ScanTagResponse**](ScanTagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSupplierScanTagsBySupplierScanGroupID

> []SupplierScanTagResponse GetSupplierScanTagsBySupplierScanGroupID(ctx, supplierScanGroupId).ScanId(scanId).UpdatedSince(updatedSince).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Execute()

Get tags for a supplier scan group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	asm "github.com/hexiosec/asm-sdk-go"
)

func main() {
	supplierScanGroupId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Supplier Scan Group ID
	scanId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Scan ID
	updatedSince := time.Now() // time.Time | Only return supplier scan tags updated at or after this timestamp (optional)
	limit := int32(56) // int32 | Maximum number of entries to return (optional)
	offset := int32(56) // int32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.GetSupplierScanTagsBySupplierScanGroupID(context.Background(), supplierScanGroupId).ScanId(scanId).UpdatedSince(updatedSince).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.GetSupplierScanTagsBySupplierScanGroupID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSupplierScanTagsBySupplierScanGroupID`: []SupplierScanTagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.GetSupplierScanTagsBySupplierScanGroupID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**supplierScanGroupId** | **string** | Supplier Scan Group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSupplierScanTagsBySupplierScanGroupIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **scanId** | **string** | Scan ID | 
 **updatedSince** | **time.Time** | Only return supplier scan tags updated at or after this timestamp | 
 **limit** | **int32** | Maximum number of entries to return | 
 **offset** | **int32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **expand** | **[]string** | Fields to expand with additional information | 

### Return type

[**[]SupplierScanTagResponse**](SupplierScanTagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTagsByOrganisationID

> []TagResponse GetTagsByOrganisationID(ctx, orgId).Limit(limit).Offset(offset).Order(order).Dir(dir).Name(name).CreatedBy(createdBy).UpdatedBy(updatedBy).Execute()

Get tags for an organisation



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
	orgId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Organisation ID
	limit := int32(56) // int32 | Maximum number of entries to return (optional)
	offset := int32(56) // int32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	name := "name_example" // string | Filter tags by name (optional)
	createdBy := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Filter tags by creator user ID (optional)
	updatedBy := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Filter tags by updater user ID (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.GetTagsByOrganisationID(context.Background(), orgId).Limit(limit).Offset(offset).Order(order).Dir(dir).Name(name).CreatedBy(createdBy).UpdatedBy(updatedBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.GetTagsByOrganisationID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTagsByOrganisationID`: []TagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.GetTagsByOrganisationID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTagsByOrganisationIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | Maximum number of entries to return | 
 **offset** | **int32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **name** | **string** | Filter tags by name | 
 **createdBy** | **string** | Filter tags by creator user ID | 
 **updatedBy** | **string** | Filter tags by updater user ID | 

### Return type

[**[]TagResponse**](TagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTagsByOrganisationIDCount

> InlineObject GetTagsByOrganisationIDCount(ctx, orgId).Name(name).CreatedBy(createdBy).UpdatedBy(updatedBy).Execute()

Get tag count for an organisation



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
	orgId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Organisation ID
	name := "name_example" // string | Filter tags by name (optional)
	createdBy := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Filter tags by creator user ID (optional)
	updatedBy := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Filter tags by updater user ID (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.GetTagsByOrganisationIDCount(context.Background(), orgId).Name(name).CreatedBy(createdBy).UpdatedBy(updatedBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.GetTagsByOrganisationIDCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTagsByOrganisationIDCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.GetTagsByOrganisationIDCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTagsByOrganisationIDCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **name** | **string** | Filter tags by name | 
 **createdBy** | **string** | Filter tags by creator user ID | 
 **updatedBy** | **string** | Filter tags by updater user ID | 

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


## RemoveTagFromLink

> RemoveTagFromLink(ctx, linkId, tagId).Execute()

Remove a tag from a link



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
	linkId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Link ID
	tagId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Tag ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.TagsAPI.RemoveTagFromLink(context.Background(), linkId, tagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.RemoveTagFromLink``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**linkId** | **string** | Link ID | 
**tagId** | **string** | Tag ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveTagFromLinkRequest struct via the builder pattern


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


## RemoveTagFromNode

> RemoveTagFromNode(ctx, nodeId, tagId).Execute()

Remove a tag from a node



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
	nodeId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Node ID
	tagId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Tag ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.TagsAPI.RemoveTagFromNode(context.Background(), nodeId, tagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.RemoveTagFromNode``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**nodeId** | **string** | Node ID | 
**tagId** | **string** | Tag ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveTagFromNodeRequest struct via the builder pattern


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


## RemoveTagFromScan

> RemoveTagFromScan(ctx, scanId, tagId).Execute()

Remove a tag from a scan



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
	scanId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Scan ID
	tagId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Tag ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.TagsAPI.RemoveTagFromScan(context.Background(), scanId, tagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.RemoveTagFromScan``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 
**tagId** | **string** | Tag ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveTagFromScanRequest struct via the builder pattern


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


## RemoveTagFromSupplierScan

> RemoveTagFromSupplierScan(ctx, supplierScanGroupId, tagId).ScanId(scanId).Execute()

Remove a tag from a supplier scan group



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
	supplierScanGroupId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Supplier Scan Group ID
	tagId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Tag ID
	scanId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Scan ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.TagsAPI.RemoveTagFromSupplierScan(context.Background(), supplierScanGroupId, tagId).ScanId(scanId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.RemoveTagFromSupplierScan``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**supplierScanGroupId** | **string** | Supplier Scan Group ID | 
**tagId** | **string** | Tag ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveTagFromSupplierScanRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **scanId** | **string** | Scan ID | 

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


## TagExistsByOrganisationID

> bool TagExistsByOrganisationID(ctx, orgId).Name(name).ExcludeTagId(excludeTagId).Execute()

Check whether a tag exists for an organisation



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
	orgId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Organisation ID
	name := "name_example" // string | Exact tag name to check
	excludeTagId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Optional tag ID to exclude from the existence check (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.TagExistsByOrganisationID(context.Background(), orgId).Name(name).ExcludeTagId(excludeTagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.TagExistsByOrganisationID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TagExistsByOrganisationID`: bool
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.TagExistsByOrganisationID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiTagExistsByOrganisationIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **name** | **string** | Exact tag name to check | 
 **excludeTagId** | **string** | Optional tag ID to exclude from the existence check | 

### Return type

**bool**

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTagByOrganisationID

> TagResponse UpdateTagByOrganisationID(ctx, orgId, tagId).CreateTagByOrganisationIDRequest(createTagByOrganisationIDRequest).Execute()

Update a tag for an organisation



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
	orgId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Organisation ID
	tagId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Tag ID
	createTagByOrganisationIDRequest := *asm.NewCreateTagByOrganisationIDRequest("Name_example") // CreateTagByOrganisationIDRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.TagsAPI.UpdateTagByOrganisationID(context.Background(), orgId, tagId).CreateTagByOrganisationIDRequest(createTagByOrganisationIDRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TagsAPI.UpdateTagByOrganisationID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTagByOrganisationID`: TagResponse
	fmt.Fprintf(os.Stdout, "Response from `TagsAPI.UpdateTagByOrganisationID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 
**tagId** | **string** | Tag ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTagByOrganisationIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **createTagByOrganisationIDRequest** | [**CreateTagByOrganisationIDRequest**](CreateTagByOrganisationIDRequest.md) |  | 

### Return type

[**TagResponse**](TagResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

