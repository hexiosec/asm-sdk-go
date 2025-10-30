# ScanGroupResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Scan Group ID | 
**OrganisationId** | **string** | Scan Group ID | 
**Name** | **string** | Scan Group Name | 
**Created** | **time.Time** | Timestamp at which the entry was created | 
**CreatedBy** | **string** | User ID of the creator user | 
**Updated** | **time.Time** | Timestamp at which the entry was last updated | 
**UpdatedBy** | **string** | User ID of the last user to update this entry | 
**Deleted** | **bool** | True if the scan group has been marked as deleted | 
**Roles** | Pointer to **[]string** | Roles granted to the current user for this scan group if requested | [optional] 
**Groups** | Pointer to **[]string** | Groups assigned to the current user for this scan group if requested | [optional] 
**CreatedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 
**UpdatedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 

## Methods

### NewScanGroupResponse

`func NewScanGroupResponse(id string, organisationId string, name string, created time.Time, createdBy string, updated time.Time, updatedBy string, deleted bool, ) *ScanGroupResponse`

NewScanGroupResponse instantiates a new ScanGroupResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanGroupResponseWithDefaults

`func NewScanGroupResponseWithDefaults() *ScanGroupResponse`

NewScanGroupResponseWithDefaults instantiates a new ScanGroupResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanGroupResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanGroupResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanGroupResponse) SetId(v string)`

SetId sets Id field to given value.


### GetOrganisationId

`func (o *ScanGroupResponse) GetOrganisationId() string`

GetOrganisationId returns the OrganisationId field if non-nil, zero value otherwise.

### GetOrganisationIdOk

`func (o *ScanGroupResponse) GetOrganisationIdOk() (*string, bool)`

GetOrganisationIdOk returns a tuple with the OrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganisationId

`func (o *ScanGroupResponse) SetOrganisationId(v string)`

SetOrganisationId sets OrganisationId field to given value.


### GetName

`func (o *ScanGroupResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanGroupResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanGroupResponse) SetName(v string)`

SetName sets Name field to given value.


### GetCreated

`func (o *ScanGroupResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanGroupResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanGroupResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetCreatedBy

`func (o *ScanGroupResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *ScanGroupResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *ScanGroupResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetUpdated

`func (o *ScanGroupResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *ScanGroupResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *ScanGroupResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetUpdatedBy

`func (o *ScanGroupResponse) GetUpdatedBy() string`

GetUpdatedBy returns the UpdatedBy field if non-nil, zero value otherwise.

### GetUpdatedByOk

`func (o *ScanGroupResponse) GetUpdatedByOk() (*string, bool)`

GetUpdatedByOk returns a tuple with the UpdatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedBy

`func (o *ScanGroupResponse) SetUpdatedBy(v string)`

SetUpdatedBy sets UpdatedBy field to given value.


### GetDeleted

`func (o *ScanGroupResponse) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *ScanGroupResponse) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *ScanGroupResponse) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.


### GetRoles

`func (o *ScanGroupResponse) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *ScanGroupResponse) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *ScanGroupResponse) SetRoles(v []string)`

SetRoles sets Roles field to given value.

### HasRoles

`func (o *ScanGroupResponse) HasRoles() bool`

HasRoles returns a boolean if a field has been set.

### GetGroups

`func (o *ScanGroupResponse) GetGroups() []string`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *ScanGroupResponse) GetGroupsOk() (*[]string, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *ScanGroupResponse) SetGroups(v []string)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *ScanGroupResponse) HasGroups() bool`

HasGroups returns a boolean if a field has been set.

### GetCreatedByUser

`func (o *ScanGroupResponse) GetCreatedByUser() UserDetailsResponse`

GetCreatedByUser returns the CreatedByUser field if non-nil, zero value otherwise.

### GetCreatedByUserOk

`func (o *ScanGroupResponse) GetCreatedByUserOk() (*UserDetailsResponse, bool)`

GetCreatedByUserOk returns a tuple with the CreatedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedByUser

`func (o *ScanGroupResponse) SetCreatedByUser(v UserDetailsResponse)`

SetCreatedByUser sets CreatedByUser field to given value.

### HasCreatedByUser

`func (o *ScanGroupResponse) HasCreatedByUser() bool`

HasCreatedByUser returns a boolean if a field has been set.

### GetUpdatedByUser

`func (o *ScanGroupResponse) GetUpdatedByUser() UserDetailsResponse`

GetUpdatedByUser returns the UpdatedByUser field if non-nil, zero value otherwise.

### GetUpdatedByUserOk

`func (o *ScanGroupResponse) GetUpdatedByUserOk() (*UserDetailsResponse, bool)`

GetUpdatedByUserOk returns a tuple with the UpdatedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedByUser

`func (o *ScanGroupResponse) SetUpdatedByUser(v UserDetailsResponse)`

SetUpdatedByUser sets UpdatedByUser field to given value.

### HasUpdatedByUser

`func (o *ScanGroupResponse) HasUpdatedByUser() bool`

HasUpdatedByUser returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


