# OrganisationResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Organisation ID | 
**Name** | **string** | Organisation Name | 
**Tier** | **string** | Organisation tier | 
**Attributes** | **map[string]interface{}** | Configuration attributes for the organisation | 
**OwnerId** | **string** | User ID of the organisation owner | 
**EmailSuffixes** | Pointer to **[]string** | Email suffixes for the organisation | [optional] 
**Deleted** | **bool** | True if the organisation has been marked as deleted | 
**Created** | **time.Time** | Timestamp at which the entry was created | 
**CreatedBy** | **string** | User ID of the creator user | 
**Updated** | **time.Time** | Timestamp at which the entry was last updated | 
**UpdatedBy** | **string** | User ID of the last user to update this entry | 
**Roles** | Pointer to **[]string** | Roles granted to the current user for this organisation if requested | [optional] 
**Groups** | Pointer to **[]string** | Groups assigned to the current user for this organisation if requested | [optional] 
**OwnerUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 
**CreatedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 

## Methods

### NewOrganisationResponse

`func NewOrganisationResponse(id string, name string, tier string, attributes map[string]interface{}, ownerId string, deleted bool, created time.Time, createdBy string, updated time.Time, updatedBy string, ) *OrganisationResponse`

NewOrganisationResponse instantiates a new OrganisationResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrganisationResponseWithDefaults

`func NewOrganisationResponseWithDefaults() *OrganisationResponse`

NewOrganisationResponseWithDefaults instantiates a new OrganisationResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *OrganisationResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *OrganisationResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *OrganisationResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *OrganisationResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *OrganisationResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *OrganisationResponse) SetName(v string)`

SetName sets Name field to given value.


### GetTier

`func (o *OrganisationResponse) GetTier() string`

GetTier returns the Tier field if non-nil, zero value otherwise.

### GetTierOk

`func (o *OrganisationResponse) GetTierOk() (*string, bool)`

GetTierOk returns a tuple with the Tier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTier

`func (o *OrganisationResponse) SetTier(v string)`

SetTier sets Tier field to given value.


### GetAttributes

`func (o *OrganisationResponse) GetAttributes() map[string]interface{}`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *OrganisationResponse) GetAttributesOk() (*map[string]interface{}, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *OrganisationResponse) SetAttributes(v map[string]interface{})`

SetAttributes sets Attributes field to given value.


### GetOwnerId

`func (o *OrganisationResponse) GetOwnerId() string`

GetOwnerId returns the OwnerId field if non-nil, zero value otherwise.

### GetOwnerIdOk

`func (o *OrganisationResponse) GetOwnerIdOk() (*string, bool)`

GetOwnerIdOk returns a tuple with the OwnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnerId

`func (o *OrganisationResponse) SetOwnerId(v string)`

SetOwnerId sets OwnerId field to given value.


### GetEmailSuffixes

`func (o *OrganisationResponse) GetEmailSuffixes() []string`

GetEmailSuffixes returns the EmailSuffixes field if non-nil, zero value otherwise.

### GetEmailSuffixesOk

`func (o *OrganisationResponse) GetEmailSuffixesOk() (*[]string, bool)`

GetEmailSuffixesOk returns a tuple with the EmailSuffixes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailSuffixes

`func (o *OrganisationResponse) SetEmailSuffixes(v []string)`

SetEmailSuffixes sets EmailSuffixes field to given value.

### HasEmailSuffixes

`func (o *OrganisationResponse) HasEmailSuffixes() bool`

HasEmailSuffixes returns a boolean if a field has been set.

### GetDeleted

`func (o *OrganisationResponse) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *OrganisationResponse) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *OrganisationResponse) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.


### GetCreated

`func (o *OrganisationResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *OrganisationResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *OrganisationResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetCreatedBy

`func (o *OrganisationResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *OrganisationResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *OrganisationResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetUpdated

`func (o *OrganisationResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *OrganisationResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *OrganisationResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetUpdatedBy

`func (o *OrganisationResponse) GetUpdatedBy() string`

GetUpdatedBy returns the UpdatedBy field if non-nil, zero value otherwise.

### GetUpdatedByOk

`func (o *OrganisationResponse) GetUpdatedByOk() (*string, bool)`

GetUpdatedByOk returns a tuple with the UpdatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedBy

`func (o *OrganisationResponse) SetUpdatedBy(v string)`

SetUpdatedBy sets UpdatedBy field to given value.


### GetRoles

`func (o *OrganisationResponse) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *OrganisationResponse) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *OrganisationResponse) SetRoles(v []string)`

SetRoles sets Roles field to given value.

### HasRoles

`func (o *OrganisationResponse) HasRoles() bool`

HasRoles returns a boolean if a field has been set.

### GetGroups

`func (o *OrganisationResponse) GetGroups() []string`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *OrganisationResponse) GetGroupsOk() (*[]string, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *OrganisationResponse) SetGroups(v []string)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *OrganisationResponse) HasGroups() bool`

HasGroups returns a boolean if a field has been set.

### GetOwnerUser

`func (o *OrganisationResponse) GetOwnerUser() UserDetailsResponse`

GetOwnerUser returns the OwnerUser field if non-nil, zero value otherwise.

### GetOwnerUserOk

`func (o *OrganisationResponse) GetOwnerUserOk() (*UserDetailsResponse, bool)`

GetOwnerUserOk returns a tuple with the OwnerUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnerUser

`func (o *OrganisationResponse) SetOwnerUser(v UserDetailsResponse)`

SetOwnerUser sets OwnerUser field to given value.

### HasOwnerUser

`func (o *OrganisationResponse) HasOwnerUser() bool`

HasOwnerUser returns a boolean if a field has been set.

### GetCreatedByUser

`func (o *OrganisationResponse) GetCreatedByUser() UserDetailsResponse`

GetCreatedByUser returns the CreatedByUser field if non-nil, zero value otherwise.

### GetCreatedByUserOk

`func (o *OrganisationResponse) GetCreatedByUserOk() (*UserDetailsResponse, bool)`

GetCreatedByUserOk returns a tuple with the CreatedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedByUser

`func (o *OrganisationResponse) SetCreatedByUser(v UserDetailsResponse)`

SetCreatedByUser sets CreatedByUser field to given value.

### HasCreatedByUser

`func (o *OrganisationResponse) HasCreatedByUser() bool`

HasCreatedByUser returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


