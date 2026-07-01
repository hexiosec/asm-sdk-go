# ReportResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Report ID | 
**ScanId** | Pointer to **string** | Scan ID | [optional] 
**OrganisationId** | Pointer to **string** | Organisation ID for organisation-scoped reports | [optional] 
**ScanName** | Pointer to **string** | Scan name | [optional] 
**IterationId** | Pointer to **string** | Iteration ID | [optional] 
**State** | [**ReportState**](ReportState.md) |  | 
**Type** | [**ReportType**](ReportType.md) |  | 
**DisplayName** | **string** | Report display name | 
**FileName** | Pointer to **string** | Report file name | [optional] 
**TemplateId** | Pointer to **string** | Report template ID used (for templated report types) | [optional] 
**Created** | **time.Time** | Report created date | 
**Updated** | **time.Time** | Report last updated date | 
**DownloadUrl** | Pointer to **string** | Will only be present when the report is done. Expires after 60s. | [optional] 
**CanManage** | Pointer to **bool** | User has \&quot;scans.reports:manage\&quot; role for this report | [optional] 

## Methods

### NewReportResponse

`func NewReportResponse(id string, state ReportState, type_ ReportType, displayName string, created time.Time, updated time.Time, ) *ReportResponse`

NewReportResponse instantiates a new ReportResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReportResponseWithDefaults

`func NewReportResponseWithDefaults() *ReportResponse`

NewReportResponseWithDefaults instantiates a new ReportResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ReportResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ReportResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ReportResponse) SetId(v string)`

SetId sets Id field to given value.


### GetScanId

`func (o *ReportResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *ReportResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *ReportResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.

### HasScanId

`func (o *ReportResponse) HasScanId() bool`

HasScanId returns a boolean if a field has been set.

### GetOrganisationId

`func (o *ReportResponse) GetOrganisationId() string`

GetOrganisationId returns the OrganisationId field if non-nil, zero value otherwise.

### GetOrganisationIdOk

`func (o *ReportResponse) GetOrganisationIdOk() (*string, bool)`

GetOrganisationIdOk returns a tuple with the OrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganisationId

`func (o *ReportResponse) SetOrganisationId(v string)`

SetOrganisationId sets OrganisationId field to given value.

### HasOrganisationId

`func (o *ReportResponse) HasOrganisationId() bool`

HasOrganisationId returns a boolean if a field has been set.

### GetScanName

`func (o *ReportResponse) GetScanName() string`

GetScanName returns the ScanName field if non-nil, zero value otherwise.

### GetScanNameOk

`func (o *ReportResponse) GetScanNameOk() (*string, bool)`

GetScanNameOk returns a tuple with the ScanName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanName

`func (o *ReportResponse) SetScanName(v string)`

SetScanName sets ScanName field to given value.

### HasScanName

`func (o *ReportResponse) HasScanName() bool`

HasScanName returns a boolean if a field has been set.

### GetIterationId

`func (o *ReportResponse) GetIterationId() string`

GetIterationId returns the IterationId field if non-nil, zero value otherwise.

### GetIterationIdOk

`func (o *ReportResponse) GetIterationIdOk() (*string, bool)`

GetIterationIdOk returns a tuple with the IterationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIterationId

`func (o *ReportResponse) SetIterationId(v string)`

SetIterationId sets IterationId field to given value.

### HasIterationId

`func (o *ReportResponse) HasIterationId() bool`

HasIterationId returns a boolean if a field has been set.

### GetState

`func (o *ReportResponse) GetState() ReportState`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ReportResponse) GetStateOk() (*ReportState, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ReportResponse) SetState(v ReportState)`

SetState sets State field to given value.


### GetType

`func (o *ReportResponse) GetType() ReportType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ReportResponse) GetTypeOk() (*ReportType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ReportResponse) SetType(v ReportType)`

SetType sets Type field to given value.


### GetDisplayName

`func (o *ReportResponse) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *ReportResponse) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *ReportResponse) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetFileName

`func (o *ReportResponse) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *ReportResponse) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *ReportResponse) SetFileName(v string)`

SetFileName sets FileName field to given value.

### HasFileName

`func (o *ReportResponse) HasFileName() bool`

HasFileName returns a boolean if a field has been set.

### GetTemplateId

`func (o *ReportResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *ReportResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *ReportResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *ReportResponse) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetCreated

`func (o *ReportResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ReportResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ReportResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetUpdated

`func (o *ReportResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *ReportResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *ReportResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetDownloadUrl

`func (o *ReportResponse) GetDownloadUrl() string`

GetDownloadUrl returns the DownloadUrl field if non-nil, zero value otherwise.

### GetDownloadUrlOk

`func (o *ReportResponse) GetDownloadUrlOk() (*string, bool)`

GetDownloadUrlOk returns a tuple with the DownloadUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDownloadUrl

`func (o *ReportResponse) SetDownloadUrl(v string)`

SetDownloadUrl sets DownloadUrl field to given value.

### HasDownloadUrl

`func (o *ReportResponse) HasDownloadUrl() bool`

HasDownloadUrl returns a boolean if a field has been set.

### GetCanManage

`func (o *ReportResponse) GetCanManage() bool`

GetCanManage returns the CanManage field if non-nil, zero value otherwise.

### GetCanManageOk

`func (o *ReportResponse) GetCanManageOk() (*bool, bool)`

GetCanManageOk returns a tuple with the CanManage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanManage

`func (o *ReportResponse) SetCanManage(v bool)`

SetCanManage sets CanManage field to given value.

### HasCanManage

`func (o *ReportResponse) HasCanManage() bool`

HasCanManage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


