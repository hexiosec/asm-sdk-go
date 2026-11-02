# ScanTagResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ScanId** | **string** | Scan ID | 
**TagId** | **string** | Tag ID | 
**CreatedAt** | **time.Time** | Timestamp at which the tag was added to the scan | 
**CreatedBy** | **string** | User ID of the creator | 
**UpdatedAt** | **time.Time** | Timestamp at which the scan tag was last updated | 
**UpdatedBy** | **string** | User ID of the last updater | 
**TagName** | Pointer to **string** | Tag Name | [optional] 
**Colour** | Pointer to **string** | Optional tag colour as a hex value | [optional] 

## Methods

### NewScanTagResponse

`func NewScanTagResponse(scanId string, tagId string, createdAt time.Time, createdBy string, updatedAt time.Time, updatedBy string, ) *ScanTagResponse`

NewScanTagResponse instantiates a new ScanTagResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanTagResponseWithDefaults

`func NewScanTagResponseWithDefaults() *ScanTagResponse`

NewScanTagResponseWithDefaults instantiates a new ScanTagResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetScanId

`func (o *ScanTagResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *ScanTagResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *ScanTagResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetTagId

`func (o *ScanTagResponse) GetTagId() string`

GetTagId returns the TagId field if non-nil, zero value otherwise.

### GetTagIdOk

`func (o *ScanTagResponse) GetTagIdOk() (*string, bool)`

GetTagIdOk returns a tuple with the TagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagId

`func (o *ScanTagResponse) SetTagId(v string)`

SetTagId sets TagId field to given value.


### GetCreatedAt

`func (o *ScanTagResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ScanTagResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ScanTagResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetCreatedBy

`func (o *ScanTagResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *ScanTagResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *ScanTagResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetUpdatedAt

`func (o *ScanTagResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *ScanTagResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *ScanTagResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetUpdatedBy

`func (o *ScanTagResponse) GetUpdatedBy() string`

GetUpdatedBy returns the UpdatedBy field if non-nil, zero value otherwise.

### GetUpdatedByOk

`func (o *ScanTagResponse) GetUpdatedByOk() (*string, bool)`

GetUpdatedByOk returns a tuple with the UpdatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedBy

`func (o *ScanTagResponse) SetUpdatedBy(v string)`

SetUpdatedBy sets UpdatedBy field to given value.


### GetTagName

`func (o *ScanTagResponse) GetTagName() string`

GetTagName returns the TagName field if non-nil, zero value otherwise.

### GetTagNameOk

`func (o *ScanTagResponse) GetTagNameOk() (*string, bool)`

GetTagNameOk returns a tuple with the TagName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagName

`func (o *ScanTagResponse) SetTagName(v string)`

SetTagName sets TagName field to given value.

### HasTagName

`func (o *ScanTagResponse) HasTagName() bool`

HasTagName returns a boolean if a field has been set.

### GetColour

`func (o *ScanTagResponse) GetColour() string`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *ScanTagResponse) GetColourOk() (*string, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *ScanTagResponse) SetColour(v string)`

SetColour sets Colour field to given value.

### HasColour

`func (o *ScanTagResponse) HasColour() bool`

HasColour returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


