# SupplierScanTagResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SupplierScanGroupId** | **string** | Supplier Scan Group ID | 
**ScanId** | **string** | Scan ID | 
**TagId** | **string** | Tag ID | 
**CreatedAt** | **time.Time** | Timestamp at which the tag was added to the supplier scan group | 
**CreatedBy** | **string** | User ID of the creator | 
**UpdatedAt** | **time.Time** | Timestamp at which the supplier scan tag was last updated | 
**UpdatedBy** | **string** | User ID of the last updater | 
**TagName** | Pointer to **string** | Tag Name | [optional] 
**Colour** | Pointer to **string** | Optional tag colour as a hex value | [optional] 

## Methods

### NewSupplierScanTagResponse

`func NewSupplierScanTagResponse(supplierScanGroupId string, scanId string, tagId string, createdAt time.Time, createdBy string, updatedAt time.Time, updatedBy string, ) *SupplierScanTagResponse`

NewSupplierScanTagResponse instantiates a new SupplierScanTagResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSupplierScanTagResponseWithDefaults

`func NewSupplierScanTagResponseWithDefaults() *SupplierScanTagResponse`

NewSupplierScanTagResponseWithDefaults instantiates a new SupplierScanTagResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSupplierScanGroupId

`func (o *SupplierScanTagResponse) GetSupplierScanGroupId() string`

GetSupplierScanGroupId returns the SupplierScanGroupId field if non-nil, zero value otherwise.

### GetSupplierScanGroupIdOk

`func (o *SupplierScanTagResponse) GetSupplierScanGroupIdOk() (*string, bool)`

GetSupplierScanGroupIdOk returns a tuple with the SupplierScanGroupId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupplierScanGroupId

`func (o *SupplierScanTagResponse) SetSupplierScanGroupId(v string)`

SetSupplierScanGroupId sets SupplierScanGroupId field to given value.


### GetScanId

`func (o *SupplierScanTagResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *SupplierScanTagResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *SupplierScanTagResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetTagId

`func (o *SupplierScanTagResponse) GetTagId() string`

GetTagId returns the TagId field if non-nil, zero value otherwise.

### GetTagIdOk

`func (o *SupplierScanTagResponse) GetTagIdOk() (*string, bool)`

GetTagIdOk returns a tuple with the TagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagId

`func (o *SupplierScanTagResponse) SetTagId(v string)`

SetTagId sets TagId field to given value.


### GetCreatedAt

`func (o *SupplierScanTagResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SupplierScanTagResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SupplierScanTagResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetCreatedBy

`func (o *SupplierScanTagResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *SupplierScanTagResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *SupplierScanTagResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetUpdatedAt

`func (o *SupplierScanTagResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *SupplierScanTagResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *SupplierScanTagResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetUpdatedBy

`func (o *SupplierScanTagResponse) GetUpdatedBy() string`

GetUpdatedBy returns the UpdatedBy field if non-nil, zero value otherwise.

### GetUpdatedByOk

`func (o *SupplierScanTagResponse) GetUpdatedByOk() (*string, bool)`

GetUpdatedByOk returns a tuple with the UpdatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedBy

`func (o *SupplierScanTagResponse) SetUpdatedBy(v string)`

SetUpdatedBy sets UpdatedBy field to given value.


### GetTagName

`func (o *SupplierScanTagResponse) GetTagName() string`

GetTagName returns the TagName field if non-nil, zero value otherwise.

### GetTagNameOk

`func (o *SupplierScanTagResponse) GetTagNameOk() (*string, bool)`

GetTagNameOk returns a tuple with the TagName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagName

`func (o *SupplierScanTagResponse) SetTagName(v string)`

SetTagName sets TagName field to given value.

### HasTagName

`func (o *SupplierScanTagResponse) HasTagName() bool`

HasTagName returns a boolean if a field has been set.

### GetColour

`func (o *SupplierScanTagResponse) GetColour() string`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *SupplierScanTagResponse) GetColourOk() (*string, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *SupplierScanTagResponse) SetColour(v string)`

SetColour sets Colour field to given value.

### HasColour

`func (o *SupplierScanTagResponse) HasColour() bool`

HasColour returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


