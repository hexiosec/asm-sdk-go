# \ActionsAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetActionByID**](ActionsAPI.md#GetActionByID) | **Get** /v1/actions/{id} | Get an action by ID
[**GetActions**](ActionsAPI.md#GetActions) | **Get** /v1/actions | Get the actions for a specified scan or scan group
[**GetRisksByActionID**](ActionsAPI.md#GetRisksByActionID) | **Get** /v1/actions/{id}/risks | Get the open risks associated with an action. Actions that are resolved will not return any risks.



## GetActionByID

> ActionResponse GetActionByID(ctx, id).Expand(expand).Lang(lang).Execute()

Get an action by ID



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
	id := "id_example" // string | Action ID
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information:  * `links` - Expand instances of the risks under this action. DEPRECATED * `link_ids` - Same as `links` except only the IDs are returned. DEPRECATED * `link_from` - Node where the risk was found. DEPRECATED * `link_to` - Node which represents the risk. DEPRECATED * `target` - Node which carries this action. DEPRECATED * `assignee_user` - User to whom this action is assigned * `modified_by` - User to last update this action * `note_modified_by` - User to last update the note against this action  (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.GetActionByID(context.Background(), id).Expand(expand).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.GetActionByID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetActionByID`: ActionResponse
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.GetActionByID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Action ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetActionByIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **expand** | **[]string** | Fields to expand with additional information:  * &#x60;links&#x60; - Expand instances of the risks under this action. DEPRECATED * &#x60;link_ids&#x60; - Same as &#x60;links&#x60; except only the IDs are returned. DEPRECATED * &#x60;link_from&#x60; - Node where the risk was found. DEPRECATED * &#x60;link_to&#x60; - Node which represents the risk. DEPRECATED * &#x60;target&#x60; - Node which carries this action. DEPRECATED * &#x60;assignee_user&#x60; - User to whom this action is assigned * &#x60;modified_by&#x60; - User to last update this action * &#x60;note_modified_by&#x60; - User to last update the note against this action  | 
 **lang** | **string** | Language of text | 

### Return type

[**ActionResponse**](ActionResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetActions

> []ActionResponse GetActions(ctx).ScanId(scanId).ScanGroupId(scanGroupId).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).IncludeOutOfScope(includeOutOfScope).IncludeSecondary(includeSecondary).Lang(lang).Execute()

Get the actions for a specified scan or scan group



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
	scanId := "scanId_example" // string | Scan ID (optional)
	scanGroupId := "scanGroupId_example" // string | Scan Group ID (required if Scan ID is not provided) (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	expand := []string{"Expand_example"} // []string | Fields to expand with additional information:  * `links` - Expand instances of the risks under this action. DEPRECATED * `link_ids` - Same as `links` except only the IDs are returned. DEPRECATED * `link_from` - Node where the risk was found (requires `links` to be expanded). DEPRECATED * `link_to` - Node which represents the risk (requires `links` to be expanded). DEPRECATED * `target` - Node which carries this action. DEPRECATED * `assignee_user` - User to whom this action is assigned * `modified_by` - User to last update this action * `note_modified_by` - User to last update the note against this action  (optional)
	includeOutOfScope := true // bool | If set, return actions with out_of_scope set to false DEPRECATED - Use include_secondary (optional)
	includeSecondary := true // bool | If set, returns primary and secondary actions (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.GetActions(context.Background()).ScanId(scanId).ScanGroupId(scanGroupId).Limit(limit).Offset(offset).Order(order).Dir(dir).Expand(expand).IncludeOutOfScope(includeOutOfScope).IncludeSecondary(includeSecondary).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.GetActions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetActions`: []ActionResponse
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.GetActions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetActionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scanId** | **string** | Scan ID | 
 **scanGroupId** | **string** | Scan Group ID (required if Scan ID is not provided) | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **expand** | **[]string** | Fields to expand with additional information:  * &#x60;links&#x60; - Expand instances of the risks under this action. DEPRECATED * &#x60;link_ids&#x60; - Same as &#x60;links&#x60; except only the IDs are returned. DEPRECATED * &#x60;link_from&#x60; - Node where the risk was found (requires &#x60;links&#x60; to be expanded). DEPRECATED * &#x60;link_to&#x60; - Node which represents the risk (requires &#x60;links&#x60; to be expanded). DEPRECATED * &#x60;target&#x60; - Node which carries this action. DEPRECATED * &#x60;assignee_user&#x60; - User to whom this action is assigned * &#x60;modified_by&#x60; - User to last update this action * &#x60;note_modified_by&#x60; - User to last update the note against this action  | 
 **includeOutOfScope** | **bool** | If set, return actions with out_of_scope set to false DEPRECATED - Use include_secondary | 
 **includeSecondary** | **bool** | If set, returns primary and secondary actions | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ActionResponse**](ActionResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetRisksByActionID

> []ScanDataRiskResponse GetRisksByActionID(ctx, id).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get the open risks associated with an action. Actions that are resolved will not return any risks.



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
	id := "id_example" // string | Action ID
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.GetRisksByActionID(context.Background(), id).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.GetRisksByActionID``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRisksByActionID`: []ScanDataRiskResponse
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.GetRisksByActionID`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Action ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRisksByActionIDRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataRiskResponse**](ScanDataRiskResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

