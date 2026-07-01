# ScanLinkTagResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LinkId** | **string** | Link ID | 
**TagId** | **string** | Tag ID | 
**Deleted** | **bool** | Whether the link tag has been soft deleted | 
**CreatedAt** | **time.Time** | Timestamp at which the tag was added to the link | 
**CreatedBy** | **string** | User ID of the creator | 
**UpdatedAt** | **time.Time** | Timestamp at which the link tag was last updated | 
**UpdatedBy** | **string** | User ID of the last updater | 
**Link** | Pointer to [**ScanLinkResponse**](ScanLinkResponse.md) |  | [optional] 
**Tag** | Pointer to [**TagResponse**](TagResponse.md) |  | [optional] 
**CreatedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 
**UpdatedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 
**TagName** | Pointer to **string** | Tag Name | [optional] 
**Colour** | Pointer to **string** | Optional tag colour as a hex value | [optional] 

## Methods

### NewScanLinkTagResponse

`func NewScanLinkTagResponse(linkId string, tagId string, deleted bool, createdAt time.Time, createdBy string, updatedAt time.Time, updatedBy string, ) *ScanLinkTagResponse`

NewScanLinkTagResponse instantiates a new ScanLinkTagResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanLinkTagResponseWithDefaults

`func NewScanLinkTagResponseWithDefaults() *ScanLinkTagResponse`

NewScanLinkTagResponseWithDefaults instantiates a new ScanLinkTagResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLinkId

`func (o *ScanLinkTagResponse) GetLinkId() string`

GetLinkId returns the LinkId field if non-nil, zero value otherwise.

### GetLinkIdOk

`func (o *ScanLinkTagResponse) GetLinkIdOk() (*string, bool)`

GetLinkIdOk returns a tuple with the LinkId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinkId

`func (o *ScanLinkTagResponse) SetLinkId(v string)`

SetLinkId sets LinkId field to given value.


### GetTagId

`func (o *ScanLinkTagResponse) GetTagId() string`

GetTagId returns the TagId field if non-nil, zero value otherwise.

### GetTagIdOk

`func (o *ScanLinkTagResponse) GetTagIdOk() (*string, bool)`

GetTagIdOk returns a tuple with the TagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagId

`func (o *ScanLinkTagResponse) SetTagId(v string)`

SetTagId sets TagId field to given value.


### GetDeleted

`func (o *ScanLinkTagResponse) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *ScanLinkTagResponse) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *ScanLinkTagResponse) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.


### GetCreatedAt

`func (o *ScanLinkTagResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ScanLinkTagResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ScanLinkTagResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetCreatedBy

`func (o *ScanLinkTagResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *ScanLinkTagResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *ScanLinkTagResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetUpdatedAt

`func (o *ScanLinkTagResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *ScanLinkTagResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *ScanLinkTagResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetUpdatedBy

`func (o *ScanLinkTagResponse) GetUpdatedBy() string`

GetUpdatedBy returns the UpdatedBy field if non-nil, zero value otherwise.

### GetUpdatedByOk

`func (o *ScanLinkTagResponse) GetUpdatedByOk() (*string, bool)`

GetUpdatedByOk returns a tuple with the UpdatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedBy

`func (o *ScanLinkTagResponse) SetUpdatedBy(v string)`

SetUpdatedBy sets UpdatedBy field to given value.


### GetLink

`func (o *ScanLinkTagResponse) GetLink() ScanLinkResponse`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *ScanLinkTagResponse) GetLinkOk() (*ScanLinkResponse, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *ScanLinkTagResponse) SetLink(v ScanLinkResponse)`

SetLink sets Link field to given value.

### HasLink

`func (o *ScanLinkTagResponse) HasLink() bool`

HasLink returns a boolean if a field has been set.

### GetTag

`func (o *ScanLinkTagResponse) GetTag() TagResponse`

GetTag returns the Tag field if non-nil, zero value otherwise.

### GetTagOk

`func (o *ScanLinkTagResponse) GetTagOk() (*TagResponse, bool)`

GetTagOk returns a tuple with the Tag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTag

`func (o *ScanLinkTagResponse) SetTag(v TagResponse)`

SetTag sets Tag field to given value.

### HasTag

`func (o *ScanLinkTagResponse) HasTag() bool`

HasTag returns a boolean if a field has been set.

### GetCreatedByUser

`func (o *ScanLinkTagResponse) GetCreatedByUser() UserDetailsResponse`

GetCreatedByUser returns the CreatedByUser field if non-nil, zero value otherwise.

### GetCreatedByUserOk

`func (o *ScanLinkTagResponse) GetCreatedByUserOk() (*UserDetailsResponse, bool)`

GetCreatedByUserOk returns a tuple with the CreatedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedByUser

`func (o *ScanLinkTagResponse) SetCreatedByUser(v UserDetailsResponse)`

SetCreatedByUser sets CreatedByUser field to given value.

### HasCreatedByUser

`func (o *ScanLinkTagResponse) HasCreatedByUser() bool`

HasCreatedByUser returns a boolean if a field has been set.

### GetUpdatedByUser

`func (o *ScanLinkTagResponse) GetUpdatedByUser() UserDetailsResponse`

GetUpdatedByUser returns the UpdatedByUser field if non-nil, zero value otherwise.

### GetUpdatedByUserOk

`func (o *ScanLinkTagResponse) GetUpdatedByUserOk() (*UserDetailsResponse, bool)`

GetUpdatedByUserOk returns a tuple with the UpdatedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedByUser

`func (o *ScanLinkTagResponse) SetUpdatedByUser(v UserDetailsResponse)`

SetUpdatedByUser sets UpdatedByUser field to given value.

### HasUpdatedByUser

`func (o *ScanLinkTagResponse) HasUpdatedByUser() bool`

HasUpdatedByUser returns a boolean if a field has been set.

### GetTagName

`func (o *ScanLinkTagResponse) GetTagName() string`

GetTagName returns the TagName field if non-nil, zero value otherwise.

### GetTagNameOk

`func (o *ScanLinkTagResponse) GetTagNameOk() (*string, bool)`

GetTagNameOk returns a tuple with the TagName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagName

`func (o *ScanLinkTagResponse) SetTagName(v string)`

SetTagName sets TagName field to given value.

### HasTagName

`func (o *ScanLinkTagResponse) HasTagName() bool`

HasTagName returns a boolean if a field has been set.

### GetColour

`func (o *ScanLinkTagResponse) GetColour() string`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *ScanLinkTagResponse) GetColourOk() (*string, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *ScanLinkTagResponse) SetColour(v string)`

SetColour sets Colour field to given value.

### HasColour

`func (o *ScanLinkTagResponse) HasColour() bool`

HasColour returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


