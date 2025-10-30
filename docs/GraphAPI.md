# \GraphAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**UpdateNodeById**](GraphAPI.md#UpdateNodeById) | **Patch** /v1/graph/nodes/{id} | Update a node by ID



## UpdateNodeById

> GenericGraphNode UpdateNodeById(ctx, id).UpdateNodeRequest(updateNodeRequest).Execute()

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
	id := "id_example" // string | Node ID
	updateNodeRequest := *asm.NewUpdateNodeRequest() // UpdateNodeRequest | Parameters to update the node

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.GraphAPI.UpdateNodeById(context.Background(), id).UpdateNodeRequest(updateNodeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GraphAPI.UpdateNodeById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateNodeById`: GenericGraphNode
	fmt.Fprintf(os.Stdout, "Response from `GraphAPI.UpdateNodeById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Node ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateNodeByIdRequest struct via the builder pattern


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

