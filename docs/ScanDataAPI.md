# \ScanDataAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetScanDataComponents**](ScanDataAPI.md#GetScanDataComponents) | **Get** /v1/scan_data/{scan_id}/components | Get components by Scan ID
[**GetScanDataComponentsCount**](ScanDataAPI.md#GetScanDataComponentsCount) | **Get** /v1/scan_data/{scan_id}/components/count | Get count of components by Scan ID
[**GetScanDataDomains**](ScanDataAPI.md#GetScanDataDomains) | **Get** /v1/scan_data/{scan_id}/domains | Get primary domains by Scan ID
[**GetScanDataDomainsCount**](ScanDataAPI.md#GetScanDataDomainsCount) | **Get** /v1/scan_data/{scan_id}/domains/count | Get count of primary domains by Scan ID
[**GetScanDataIPs**](ScanDataAPI.md#GetScanDataIPs) | **Get** /v1/scan_data/{scan_id}/ips | Get primary IPs by Scan ID
[**GetScanDataIPsCount**](ScanDataAPI.md#GetScanDataIPsCount) | **Get** /v1/scan_data/{scan_id}/ips/count | Get count of primary IPs by Scan ID
[**GetScanDataLinkChanges**](ScanDataAPI.md#GetScanDataLinkChanges) | **Get** /v1/scan_data/{scan_id}/link_changes | Get link changes by Scan ID and iteration(s)
[**GetScanDataOutOfScopeDomains**](ScanDataAPI.md#GetScanDataOutOfScopeDomains) | **Get** /v1/scan_data/{scan_id}/out_of_scope_domains | Get out-of-scope domains by Scan ID
[**GetScanDataOutOfScopeDomainsCount**](ScanDataAPI.md#GetScanDataOutOfScopeDomainsCount) | **Get** /v1/scan_data/{scan_id}/out_of_scope_domains/count | Get count of out-of-scope domains by Scan ID
[**GetScanDataRisks**](ScanDataAPI.md#GetScanDataRisks) | **Get** /v1/scan_data/{scan_id}/risks | Get risks by Scan ID
[**GetScanDataRisksCount**](ScanDataAPI.md#GetScanDataRisksCount) | **Get** /v1/scan_data/{scan_id}/risks/count | Get count of risks by Scan ID
[**GetScanDataSecondaryDomains**](ScanDataAPI.md#GetScanDataSecondaryDomains) | **Get** /v1/scan_data/{scan_id}/secondary_domains | Get secondary domains by Scan ID
[**GetScanDataSecondaryDomainsCount**](ScanDataAPI.md#GetScanDataSecondaryDomainsCount) | **Get** /v1/scan_data/{scan_id}/secondary_domains/count | Get count of secondary domains by Scan ID
[**GetScanDataServices**](ScanDataAPI.md#GetScanDataServices) | **Get** /v1/scan_data/{scan_id}/services | Get services by Scan ID
[**GetScanDataServicesCount**](ScanDataAPI.md#GetScanDataServicesCount) | **Get** /v1/scan_data/{scan_id}/services/count | Get count of services by Scan ID
[**GetScanDataWebPresence**](ScanDataAPI.md#GetScanDataWebPresence) | **Get** /v1/scan_data/{scan_id}/web_presence | Get primary web presence URLs by Scan ID
[**GetScanDataWebPresenceCount**](ScanDataAPI.md#GetScanDataWebPresenceCount) | **Get** /v1/scan_data/{scan_id}/web_presence/count | Get count of primary web presence URLs by Scan ID



## GetScanDataComponents

> []ScanDataComponentResponse GetScanDataComponents(ctx, scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get components by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of component IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataComponents(context.Background(), scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataComponents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataComponents`: []ScanDataComponentResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataComponents`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataComponentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of component IDs to filter by | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataComponentResponse**](ScanDataComponentResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataComponentsCount

> InlineObject GetScanDataComponentsCount(ctx, scanId).Ids(ids).Execute()

Get count of components by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of component IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataComponentsCount(context.Background(), scanId).Ids(ids).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataComponentsCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataComponentsCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataComponentsCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataComponentsCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of component IDs to filter by | 

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


## GetScanDataDomains

> []ScanDataDomainResponse GetScanDataDomains(ctx, scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get primary domains by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of domain IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataDomains(context.Background(), scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataDomains``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataDomains`: []ScanDataDomainResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataDomains`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataDomainsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of domain IDs to filter by | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataDomainResponse**](ScanDataDomainResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataDomainsCount

> InlineObject GetScanDataDomainsCount(ctx, scanId).Ids(ids).Execute()

Get count of primary domains by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of domain IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataDomainsCount(context.Background(), scanId).Ids(ids).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataDomainsCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataDomainsCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataDomainsCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataDomainsCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of domain IDs to filter by | 

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


## GetScanDataIPs

> []ScanDataIPResponse GetScanDataIPs(ctx, scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get primary IPs by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of ip IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataIPs(context.Background(), scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataIPs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataIPs`: []ScanDataIPResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataIPs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataIPsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of ip IDs to filter by | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataIPResponse**](ScanDataIPResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataIPsCount

> InlineObject GetScanDataIPsCount(ctx, scanId).Ids(ids).Execute()

Get count of primary IPs by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of ip IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataIPsCount(context.Background(), scanId).Ids(ids).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataIPsCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataIPsCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataIPsCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataIPsCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of ip IDs to filter by | 

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


## GetScanDataLinkChanges

> ScanDataLinkChangesResponse GetScanDataLinkChanges(ctx, scanId).LinkType(linkType).FromType(fromType).ToType(toType).RiskSeverityNumber(riskSeverityNumber).IncludeTransient(includeTransient).FromIteration(fromIteration).ToIteration(toIteration).LastIterations(lastIterations).Lang(lang).Execute()

Get link changes by Scan ID and iteration(s)



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
	linkType := []string{"LinkType_example"} // []string | Filter by link type (optional)
	fromType := []string{"FromType_example"} // []string | Filter by from node type (optional)
	toType := []string{"ToType_example"} // []string | Filter by to node type (optional)
	riskSeverityNumber := []int32{int32(123)} // []int32 | Filter by risk severity (optional)
	includeTransient := true // bool | Include transient link changes. A transient link is one that was added and then removed within the timeframe of the changes. (optional)
	fromIteration := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | From iteration ID (uuid) (optional)
	toIteration := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | To iteration ID (uuid) (optional)
	lastIterations := int32(56) // int32 | Number of last iterations to compare (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataLinkChanges(context.Background(), scanId).LinkType(linkType).FromType(fromType).ToType(toType).RiskSeverityNumber(riskSeverityNumber).IncludeTransient(includeTransient).FromIteration(fromIteration).ToIteration(toIteration).LastIterations(lastIterations).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataLinkChanges``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataLinkChanges`: ScanDataLinkChangesResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataLinkChanges`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataLinkChangesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **linkType** | **[]string** | Filter by link type | 
 **fromType** | **[]string** | Filter by from node type | 
 **toType** | **[]string** | Filter by to node type | 
 **riskSeverityNumber** | **[]int32** | Filter by risk severity | 
 **includeTransient** | **bool** | Include transient link changes. A transient link is one that was added and then removed within the timeframe of the changes. | 
 **fromIteration** | **string** | From iteration ID (uuid) | 
 **toIteration** | **string** | To iteration ID (uuid) | 
 **lastIterations** | **int32** | Number of last iterations to compare | 
 **lang** | **string** | Language of text | 

### Return type

[**ScanDataLinkChangesResponse**](ScanDataLinkChangesResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataOutOfScopeDomains

> []ScanDataOutOfScopeDomainResponse GetScanDataOutOfScopeDomains(ctx, scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get out-of-scope domains by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of out-of-scope domain IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataOutOfScopeDomains(context.Background(), scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataOutOfScopeDomains``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataOutOfScopeDomains`: []ScanDataOutOfScopeDomainResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataOutOfScopeDomains`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataOutOfScopeDomainsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of out-of-scope domain IDs to filter by | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataOutOfScopeDomainResponse**](ScanDataOutOfScopeDomainResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataOutOfScopeDomainsCount

> InlineObject GetScanDataOutOfScopeDomainsCount(ctx, scanId).Ids(ids).Execute()

Get count of out-of-scope domains by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of out-of-scope domain IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataOutOfScopeDomainsCount(context.Background(), scanId).Ids(ids).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataOutOfScopeDomainsCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataOutOfScopeDomainsCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataOutOfScopeDomainsCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataOutOfScopeDomainsCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of out-of-scope domain IDs to filter by | 

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


## GetScanDataRisks

> []ScanDataRiskResponse GetScanDataRisks(ctx, scanId).LinkIds(linkIds).RiskNodeIds(riskNodeIds).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get risks by Scan ID



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
	linkIds := []string{"Inner_example"} // []string | List of risk Link IDs to filter by (optional)
	riskNodeIds := []string{"Inner_example"} // []string | List of risk Node IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataRisks(context.Background(), scanId).LinkIds(linkIds).RiskNodeIds(riskNodeIds).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataRisks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataRisks`: []ScanDataRiskResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataRisks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataRisksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **linkIds** | **[]string** | List of risk Link IDs to filter by | 
 **riskNodeIds** | **[]string** | List of risk Node IDs to filter by | 
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


## GetScanDataRisksCount

> InlineObject GetScanDataRisksCount(ctx, scanId).LinkIds(linkIds).RiskNodeIds(riskNodeIds).Execute()

Get count of risks by Scan ID



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
	linkIds := []string{"Inner_example"} // []string | List of risk Link IDs to filter by (optional)
	riskNodeIds := []string{"Inner_example"} // []string | List of risk Node IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataRisksCount(context.Background(), scanId).LinkIds(linkIds).RiskNodeIds(riskNodeIds).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataRisksCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataRisksCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataRisksCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataRisksCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **linkIds** | **[]string** | List of risk Link IDs to filter by | 
 **riskNodeIds** | **[]string** | List of risk Node IDs to filter by | 

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


## GetScanDataSecondaryDomains

> []ScanDataOutOfScopeDomainResponse GetScanDataSecondaryDomains(ctx, scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get secondary domains by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of secondary domain IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataSecondaryDomains(context.Background(), scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataSecondaryDomains``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataSecondaryDomains`: []ScanDataOutOfScopeDomainResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataSecondaryDomains`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataSecondaryDomainsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of secondary domain IDs to filter by | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataOutOfScopeDomainResponse**](ScanDataOutOfScopeDomainResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataSecondaryDomainsCount

> InlineObject GetScanDataSecondaryDomainsCount(ctx, scanId).Ids(ids).Execute()

Get count of secondary domains by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of secondary domain IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataSecondaryDomainsCount(context.Background(), scanId).Ids(ids).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataSecondaryDomainsCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataSecondaryDomainsCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataSecondaryDomainsCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataSecondaryDomainsCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of secondary domain IDs to filter by | 

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


## GetScanDataServices

> []ScanDataServiceResponse GetScanDataServices(ctx, scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get services by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of service IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataServices(context.Background(), scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataServices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataServices`: []ScanDataServiceResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataServices`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataServicesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of service IDs to filter by | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataServiceResponse**](ScanDataServiceResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataServicesCount

> InlineObject GetScanDataServicesCount(ctx, scanId).Ids(ids).Execute()

Get count of services by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of service IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataServicesCount(context.Background(), scanId).Ids(ids).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataServicesCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataServicesCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataServicesCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataServicesCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of service IDs to filter by | 

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


## GetScanDataWebPresence

> []ScanDataWebPresenceResponse GetScanDataWebPresence(ctx, scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()

Get primary web presence URLs by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of URL IDs to filter by (optional)
	limit := float32(8.14) // float32 | Maximum number of entries to return (optional)
	offset := float32(8.14) // float32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)
	lang := "lang_example" // string | Language of text (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataWebPresence(context.Background(), scanId).Ids(ids).Limit(limit).Offset(offset).Order(order).Dir(dir).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataWebPresence``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataWebPresence`: []ScanDataWebPresenceResponse
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataWebPresence`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataWebPresenceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of URL IDs to filter by | 
 **limit** | **float32** | Maximum number of entries to return | 
 **offset** | **float32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 
 **lang** | **string** | Language of text | 

### Return type

[**[]ScanDataWebPresenceResponse**](ScanDataWebPresenceResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetScanDataWebPresenceCount

> InlineObject GetScanDataWebPresenceCount(ctx, scanId).Ids(ids).Execute()

Get count of primary web presence URLs by Scan ID



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
	ids := []string{"Inner_example"} // []string | List of URL IDs to filter by (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ScanDataAPI.GetScanDataWebPresenceCount(context.Background(), scanId).Ids(ids).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ScanDataAPI.GetScanDataWebPresenceCount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetScanDataWebPresenceCount`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ScanDataAPI.GetScanDataWebPresenceCount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetScanDataWebPresenceCountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ids** | **[]string** | List of URL IDs to filter by | 

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

