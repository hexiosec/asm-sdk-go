# ReportTemplateResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Report ID | 
**OrganisationId** | **string** | Organisation ID | 
**State** | [**ReportTemplateState**](ReportTemplateState.md) |  | 
**Type** | **string** | Templatable report type (subset of ReportType that use templates) | 
**DisplayName** | **string** | Report template display name | 
**FileName** | Pointer to **string** | Report template file name | [optional] 
**Created** | **time.Time** | Report template created date | 
**Updated** | **time.Time** | Report template last updated date | 
**DownloadUrl** | Pointer to **string** | Expires after 60s. | [optional] 
**UploadUrl** | Pointer to **string** | Expires after 60s. | [optional] 

## Methods

### NewReportTemplateResponse

`func NewReportTemplateResponse(id string, organisationId string, state ReportTemplateState, type_ string, displayName string, created time.Time, updated time.Time, ) *ReportTemplateResponse`

NewReportTemplateResponse instantiates a new ReportTemplateResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReportTemplateResponseWithDefaults

`func NewReportTemplateResponseWithDefaults() *ReportTemplateResponse`

NewReportTemplateResponseWithDefaults instantiates a new ReportTemplateResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ReportTemplateResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ReportTemplateResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ReportTemplateResponse) SetId(v string)`

SetId sets Id field to given value.


### GetOrganisationId

`func (o *ReportTemplateResponse) GetOrganisationId() string`

GetOrganisationId returns the OrganisationId field if non-nil, zero value otherwise.

### GetOrganisationIdOk

`func (o *ReportTemplateResponse) GetOrganisationIdOk() (*string, bool)`

GetOrganisationIdOk returns a tuple with the OrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganisationId

`func (o *ReportTemplateResponse) SetOrganisationId(v string)`

SetOrganisationId sets OrganisationId field to given value.


### GetState

`func (o *ReportTemplateResponse) GetState() ReportTemplateState`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ReportTemplateResponse) GetStateOk() (*ReportTemplateState, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ReportTemplateResponse) SetState(v ReportTemplateState)`

SetState sets State field to given value.


### GetType

`func (o *ReportTemplateResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ReportTemplateResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ReportTemplateResponse) SetType(v string)`

SetType sets Type field to given value.


### GetDisplayName

`func (o *ReportTemplateResponse) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *ReportTemplateResponse) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *ReportTemplateResponse) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetFileName

`func (o *ReportTemplateResponse) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *ReportTemplateResponse) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *ReportTemplateResponse) SetFileName(v string)`

SetFileName sets FileName field to given value.

### HasFileName

`func (o *ReportTemplateResponse) HasFileName() bool`

HasFileName returns a boolean if a field has been set.

### GetCreated

`func (o *ReportTemplateResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ReportTemplateResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ReportTemplateResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetUpdated

`func (o *ReportTemplateResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *ReportTemplateResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *ReportTemplateResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetDownloadUrl

`func (o *ReportTemplateResponse) GetDownloadUrl() string`

GetDownloadUrl returns the DownloadUrl field if non-nil, zero value otherwise.

### GetDownloadUrlOk

`func (o *ReportTemplateResponse) GetDownloadUrlOk() (*string, bool)`

GetDownloadUrlOk returns a tuple with the DownloadUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDownloadUrl

`func (o *ReportTemplateResponse) SetDownloadUrl(v string)`

SetDownloadUrl sets DownloadUrl field to given value.

### HasDownloadUrl

`func (o *ReportTemplateResponse) HasDownloadUrl() bool`

HasDownloadUrl returns a boolean if a field has been set.

### GetUploadUrl

`func (o *ReportTemplateResponse) GetUploadUrl() string`

GetUploadUrl returns the UploadUrl field if non-nil, zero value otherwise.

### GetUploadUrlOk

`func (o *ReportTemplateResponse) GetUploadUrlOk() (*string, bool)`

GetUploadUrlOk returns a tuple with the UploadUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUploadUrl

`func (o *ReportTemplateResponse) SetUploadUrl(v string)`

SetUploadUrl sets UploadUrl field to given value.

### HasUploadUrl

`func (o *ReportTemplateResponse) HasUploadUrl() bool`

HasUploadUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


