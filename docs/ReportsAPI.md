# \ReportsAPI

All URIs are relative to *https://asm.hexiosec.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateReport**](ReportsAPI.md#CreateReport) | **Post** /v1/reports | Create a report
[**DeleteReport**](ReportsAPI.md#DeleteReport) | **Delete** /v1/reports/{id} | Delete a report
[**GetReport**](ReportsAPI.md#GetReport) | **Get** /v1/reports/{id} | Get a report
[**GetReportCountForOrg**](ReportsAPI.md#GetReportCountForOrg) | **Get** /v1/reports/organisation/{org_id}/count | Get report count for an organisation
[**GetReportCountForScan**](ReportsAPI.md#GetReportCountForScan) | **Get** /v1/reports/scan/{scan_id}/count | Get report count for a scan
[**GetReportTemplatesForOrg**](ReportsAPI.md#GetReportTemplatesForOrg) | **Get** /v1/reports/templates/organisation/{org_id} | Get report templates for an organisation
[**GetReportsForOrg**](ReportsAPI.md#GetReportsForOrg) | **Get** /v1/reports/organisation/{org_id} | Get reports for an organisation
[**GetReportsForScan**](ReportsAPI.md#GetReportsForScan) | **Get** /v1/reports/scan/{scan_id} | Get reports for a scan



## CreateReport

> ReportResponse CreateReport(ctx).CreateReportRequest(createReportRequest).Execute()

Create a report



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
	createReportRequest := asm.createReport_request{CreateExcelSummaryReportBody: asm.NewCreateExcelSummaryReportBody(asm.ReportType("summary"), "ScanId_example", "Name_example")} // CreateReportRequest | 

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ReportsAPI.CreateReport(context.Background()).CreateReportRequest(createReportRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.CreateReport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateReport`: ReportResponse
	fmt.Fprintf(os.Stdout, "Response from `ReportsAPI.CreateReport`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateReportRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createReportRequest** | [**CreateReportRequest**](CreateReportRequest.md) |  | 

### Return type

[**ReportResponse**](ReportResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteReport

> DeleteReport(ctx, id).Execute()

Delete a report



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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Report ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	r, err := apiClient.ReportsAPI.DeleteReport(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.DeleteReport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Report ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteReportRequest struct via the builder pattern


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


## GetReport

> ReportResponse GetReport(ctx, id).Execute()

Get a report



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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Report ID

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ReportsAPI.GetReport(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.GetReport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetReport`: ReportResponse
	fmt.Fprintf(os.Stdout, "Response from `ReportsAPI.GetReport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Report ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReportRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ReportResponse**](ReportResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetReportCountForOrg

> InlineObject GetReportCountForOrg(ctx, orgId).Search(search).Type_(type_).TemplateId(templateId).Execute()

Get report count for an organisation



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
	search := "search_example" // string | Search term (optional)
	type_ := asm.ReportType("summary") // ReportType | Report type (optional)
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Template ID used to generate report (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ReportsAPI.GetReportCountForOrg(context.Background(), orgId).Search(search).Type_(type_).TemplateId(templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.GetReportCountForOrg``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetReportCountForOrg`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ReportsAPI.GetReportCountForOrg`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReportCountForOrgRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **search** | **string** | Search term | 
 **type_** | [**ReportType**](ReportType.md) | Report type | 
 **templateId** | **string** | Template ID used to generate report | 

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


## GetReportCountForScan

> InlineObject GetReportCountForScan(ctx, scanId).Search(search).Type_(type_).TemplateId(templateId).Execute()

Get report count for a scan



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
	search := "search_example" // string | Search term (optional)
	type_ := asm.ReportType("summary") // ReportType | Report type (optional)
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Template ID used to generate report (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ReportsAPI.GetReportCountForScan(context.Background(), scanId).Search(search).Type_(type_).TemplateId(templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.GetReportCountForScan``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetReportCountForScan`: InlineObject
	fmt.Fprintf(os.Stdout, "Response from `ReportsAPI.GetReportCountForScan`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReportCountForScanRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **search** | **string** | Search term | 
 **type_** | [**ReportType**](ReportType.md) | Report type | 
 **templateId** | **string** | Template ID used to generate report | 

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


## GetReportTemplatesForOrg

> []ReportTemplateResponse GetReportTemplatesForOrg(ctx, orgId).IncludeGlobal(includeGlobal).Execute()

Get report templates for an organisation



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
	includeGlobal := true // bool | Include global templates (`organisation_id = null`) in addition to organisation templates (optional) (default to false)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ReportsAPI.GetReportTemplatesForOrg(context.Background(), orgId).IncludeGlobal(includeGlobal).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.GetReportTemplatesForOrg``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetReportTemplatesForOrg`: []ReportTemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `ReportsAPI.GetReportTemplatesForOrg`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReportTemplatesForOrgRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **includeGlobal** | **bool** | Include global templates (&#x60;organisation_id &#x3D; null&#x60;) in addition to organisation templates | [default to false]

### Return type

[**[]ReportTemplateResponse**](ReportTemplateResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetReportsForOrg

> []ReportResponse GetReportsForOrg(ctx, orgId).Search(search).Type_(type_).TemplateId(templateId).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()

Get reports for an organisation



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
	search := "search_example" // string | Search term (optional)
	type_ := asm.ReportType("summary") // ReportType | Report type (optional)
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Template ID used to generate report (optional)
	limit := int32(56) // int32 | Maximum number of entries to return (optional)
	offset := int32(56) // int32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ReportsAPI.GetReportsForOrg(context.Background(), orgId).Search(search).Type_(type_).TemplateId(templateId).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.GetReportsForOrg``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetReportsForOrg`: []ReportResponse
	fmt.Fprintf(os.Stdout, "Response from `ReportsAPI.GetReportsForOrg`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** | Organisation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReportsForOrgRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **search** | **string** | Search term | 
 **type_** | [**ReportType**](ReportType.md) | Report type | 
 **templateId** | **string** | Template ID used to generate report | 
 **limit** | **int32** | Maximum number of entries to return | 
 **offset** | **int32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 

### Return type

[**[]ReportResponse**](ReportResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetReportsForScan

> []ReportResponse GetReportsForScan(ctx, scanId).Search(search).Type_(type_).TemplateId(templateId).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()

Get reports for a scan



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
	search := "search_example" // string | Search term (optional)
	type_ := asm.ReportType("summary") // ReportType | Report type (optional)
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Template ID used to generate report (optional)
	limit := int32(56) // int32 | Maximum number of entries to return (optional)
	offset := int32(56) // int32 | Offset into the list of entries to return (optional)
	order := "order_example" // string | Column to order results by (optional)
	dir := "dir_example" // string | Sort direction (optional)

	configuration := asm.NewConfiguration()
	apiClient := asm.NewAPIClient(configuration)
	resp, r, err := apiClient.ReportsAPI.GetReportsForScan(context.Background(), scanId).Search(search).Type_(type_).TemplateId(templateId).Limit(limit).Offset(offset).Order(order).Dir(dir).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReportsAPI.GetReportsForScan``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetReportsForScan`: []ReportResponse
	fmt.Fprintf(os.Stdout, "Response from `ReportsAPI.GetReportsForScan`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**scanId** | **string** | Scan ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReportsForScanRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **search** | **string** | Search term | 
 **type_** | [**ReportType**](ReportType.md) | Report type | 
 **templateId** | **string** | Template ID used to generate report | 
 **limit** | **int32** | Maximum number of entries to return | 
 **offset** | **int32** | Offset into the list of entries to return | 
 **order** | **string** | Column to order results by | 
 **dir** | **string** | Sort direction | 

### Return type

[**[]ReportResponse**](ReportResponse.md)

### Authorization

[APIKey](../README.md#APIKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

