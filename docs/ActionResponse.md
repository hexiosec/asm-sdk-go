# ActionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Action ID | 
**NodeId** | **string** | ID of the node against which this action is registered. Has been replaced with the asset_id param | 
**ScanId** | **string** | Scan ID | 
**AssetId** | Pointer to **string** | ID of the node against which this action is registered | [optional] 
**AssetType** | Pointer to **string** | Label of the node against which this action is registered | [optional] 
**AssetName** | Pointer to **string** | Name of the node against which this action is registered | [optional] 
**Rule** | **string** | Name of the rule that has caused this action | 
**State** | **string** | Management state of the action | 
**Name** | Pointer to **string** | Description in lang | [optional] 
**Description** | Pointer to **string** | Description in lang | [optional] 
**Remediation** | Pointer to **string** | Remediation in lang | [optional] 
**Note** | Pointer to **string** | User-supplied notes about this action | [optional] 
**Created** | **time.Time** | Timestamp at which the entry was created | 
**Modified** | Pointer to **time.Time** | Timestamp at which the entry was updated | [optional] 
**OutOfScope** | Pointer to **bool** | Deprecated – True if this action has been marked as out of scope - Use **is_secondary** | [optional] 
**IsSecondary** | Pointer to **bool** | True if this action has been marked as secondary | [optional] 
**ResolvedAt** | Pointer to **time.Time** | Timestamp at which the action was resolved | [optional] 
**Links** | Pointer to [**[]ActionLinkResponse**](ActionLinkResponse.md) | Has been replaced with the get risks endpoint | [optional] 
**LinkIds** | Pointer to **[]string** | Has been replaced with the get risks endpoint | [optional] 
**Target** | Pointer to **map[string]interface{}** | Has been replaced with the asset_* params | [optional] 
**AssigneeUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 
**ModifiedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 
**NoteModifiedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 

## Methods

### NewActionResponse

`func NewActionResponse(id string, nodeId string, scanId string, rule string, state string, created time.Time, ) *ActionResponse`

NewActionResponse instantiates a new ActionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewActionResponseWithDefaults

`func NewActionResponseWithDefaults() *ActionResponse`

NewActionResponseWithDefaults instantiates a new ActionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ActionResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ActionResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ActionResponse) SetId(v string)`

SetId sets Id field to given value.


### GetNodeId

`func (o *ActionResponse) GetNodeId() string`

GetNodeId returns the NodeId field if non-nil, zero value otherwise.

### GetNodeIdOk

`func (o *ActionResponse) GetNodeIdOk() (*string, bool)`

GetNodeIdOk returns a tuple with the NodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeId

`func (o *ActionResponse) SetNodeId(v string)`

SetNodeId sets NodeId field to given value.


### GetScanId

`func (o *ActionResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *ActionResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *ActionResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetAssetId

`func (o *ActionResponse) GetAssetId() string`

GetAssetId returns the AssetId field if non-nil, zero value otherwise.

### GetAssetIdOk

`func (o *ActionResponse) GetAssetIdOk() (*string, bool)`

GetAssetIdOk returns a tuple with the AssetId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetId

`func (o *ActionResponse) SetAssetId(v string)`

SetAssetId sets AssetId field to given value.

### HasAssetId

`func (o *ActionResponse) HasAssetId() bool`

HasAssetId returns a boolean if a field has been set.

### GetAssetType

`func (o *ActionResponse) GetAssetType() string`

GetAssetType returns the AssetType field if non-nil, zero value otherwise.

### GetAssetTypeOk

`func (o *ActionResponse) GetAssetTypeOk() (*string, bool)`

GetAssetTypeOk returns a tuple with the AssetType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetType

`func (o *ActionResponse) SetAssetType(v string)`

SetAssetType sets AssetType field to given value.

### HasAssetType

`func (o *ActionResponse) HasAssetType() bool`

HasAssetType returns a boolean if a field has been set.

### GetAssetName

`func (o *ActionResponse) GetAssetName() string`

GetAssetName returns the AssetName field if non-nil, zero value otherwise.

### GetAssetNameOk

`func (o *ActionResponse) GetAssetNameOk() (*string, bool)`

GetAssetNameOk returns a tuple with the AssetName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetName

`func (o *ActionResponse) SetAssetName(v string)`

SetAssetName sets AssetName field to given value.

### HasAssetName

`func (o *ActionResponse) HasAssetName() bool`

HasAssetName returns a boolean if a field has been set.

### GetRule

`func (o *ActionResponse) GetRule() string`

GetRule returns the Rule field if non-nil, zero value otherwise.

### GetRuleOk

`func (o *ActionResponse) GetRuleOk() (*string, bool)`

GetRuleOk returns a tuple with the Rule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRule

`func (o *ActionResponse) SetRule(v string)`

SetRule sets Rule field to given value.


### GetState

`func (o *ActionResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ActionResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ActionResponse) SetState(v string)`

SetState sets State field to given value.


### GetName

`func (o *ActionResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ActionResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ActionResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ActionResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *ActionResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ActionResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ActionResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ActionResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetRemediation

`func (o *ActionResponse) GetRemediation() string`

GetRemediation returns the Remediation field if non-nil, zero value otherwise.

### GetRemediationOk

`func (o *ActionResponse) GetRemediationOk() (*string, bool)`

GetRemediationOk returns a tuple with the Remediation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemediation

`func (o *ActionResponse) SetRemediation(v string)`

SetRemediation sets Remediation field to given value.

### HasRemediation

`func (o *ActionResponse) HasRemediation() bool`

HasRemediation returns a boolean if a field has been set.

### GetNote

`func (o *ActionResponse) GetNote() string`

GetNote returns the Note field if non-nil, zero value otherwise.

### GetNoteOk

`func (o *ActionResponse) GetNoteOk() (*string, bool)`

GetNoteOk returns a tuple with the Note field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNote

`func (o *ActionResponse) SetNote(v string)`

SetNote sets Note field to given value.

### HasNote

`func (o *ActionResponse) HasNote() bool`

HasNote returns a boolean if a field has been set.

### GetCreated

`func (o *ActionResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ActionResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ActionResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetModified

`func (o *ActionResponse) GetModified() time.Time`

GetModified returns the Modified field if non-nil, zero value otherwise.

### GetModifiedOk

`func (o *ActionResponse) GetModifiedOk() (*time.Time, bool)`

GetModifiedOk returns a tuple with the Modified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModified

`func (o *ActionResponse) SetModified(v time.Time)`

SetModified sets Modified field to given value.

### HasModified

`func (o *ActionResponse) HasModified() bool`

HasModified returns a boolean if a field has been set.

### GetOutOfScope

`func (o *ActionResponse) GetOutOfScope() bool`

GetOutOfScope returns the OutOfScope field if non-nil, zero value otherwise.

### GetOutOfScopeOk

`func (o *ActionResponse) GetOutOfScopeOk() (*bool, bool)`

GetOutOfScopeOk returns a tuple with the OutOfScope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutOfScope

`func (o *ActionResponse) SetOutOfScope(v bool)`

SetOutOfScope sets OutOfScope field to given value.

### HasOutOfScope

`func (o *ActionResponse) HasOutOfScope() bool`

HasOutOfScope returns a boolean if a field has been set.

### GetIsSecondary

`func (o *ActionResponse) GetIsSecondary() bool`

GetIsSecondary returns the IsSecondary field if non-nil, zero value otherwise.

### GetIsSecondaryOk

`func (o *ActionResponse) GetIsSecondaryOk() (*bool, bool)`

GetIsSecondaryOk returns a tuple with the IsSecondary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSecondary

`func (o *ActionResponse) SetIsSecondary(v bool)`

SetIsSecondary sets IsSecondary field to given value.

### HasIsSecondary

`func (o *ActionResponse) HasIsSecondary() bool`

HasIsSecondary returns a boolean if a field has been set.

### GetResolvedAt

`func (o *ActionResponse) GetResolvedAt() time.Time`

GetResolvedAt returns the ResolvedAt field if non-nil, zero value otherwise.

### GetResolvedAtOk

`func (o *ActionResponse) GetResolvedAtOk() (*time.Time, bool)`

GetResolvedAtOk returns a tuple with the ResolvedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResolvedAt

`func (o *ActionResponse) SetResolvedAt(v time.Time)`

SetResolvedAt sets ResolvedAt field to given value.

### HasResolvedAt

`func (o *ActionResponse) HasResolvedAt() bool`

HasResolvedAt returns a boolean if a field has been set.

### GetLinks

`func (o *ActionResponse) GetLinks() []ActionLinkResponse`

GetLinks returns the Links field if non-nil, zero value otherwise.

### GetLinksOk

`func (o *ActionResponse) GetLinksOk() (*[]ActionLinkResponse, bool)`

GetLinksOk returns a tuple with the Links field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinks

`func (o *ActionResponse) SetLinks(v []ActionLinkResponse)`

SetLinks sets Links field to given value.

### HasLinks

`func (o *ActionResponse) HasLinks() bool`

HasLinks returns a boolean if a field has been set.

### GetLinkIds

`func (o *ActionResponse) GetLinkIds() []string`

GetLinkIds returns the LinkIds field if non-nil, zero value otherwise.

### GetLinkIdsOk

`func (o *ActionResponse) GetLinkIdsOk() (*[]string, bool)`

GetLinkIdsOk returns a tuple with the LinkIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinkIds

`func (o *ActionResponse) SetLinkIds(v []string)`

SetLinkIds sets LinkIds field to given value.

### HasLinkIds

`func (o *ActionResponse) HasLinkIds() bool`

HasLinkIds returns a boolean if a field has been set.

### GetTarget

`func (o *ActionResponse) GetTarget() map[string]interface{}`

GetTarget returns the Target field if non-nil, zero value otherwise.

### GetTargetOk

`func (o *ActionResponse) GetTargetOk() (*map[string]interface{}, bool)`

GetTargetOk returns a tuple with the Target field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTarget

`func (o *ActionResponse) SetTarget(v map[string]interface{})`

SetTarget sets Target field to given value.

### HasTarget

`func (o *ActionResponse) HasTarget() bool`

HasTarget returns a boolean if a field has been set.

### GetAssigneeUser

`func (o *ActionResponse) GetAssigneeUser() UserDetailsResponse`

GetAssigneeUser returns the AssigneeUser field if non-nil, zero value otherwise.

### GetAssigneeUserOk

`func (o *ActionResponse) GetAssigneeUserOk() (*UserDetailsResponse, bool)`

GetAssigneeUserOk returns a tuple with the AssigneeUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssigneeUser

`func (o *ActionResponse) SetAssigneeUser(v UserDetailsResponse)`

SetAssigneeUser sets AssigneeUser field to given value.

### HasAssigneeUser

`func (o *ActionResponse) HasAssigneeUser() bool`

HasAssigneeUser returns a boolean if a field has been set.

### GetModifiedByUser

`func (o *ActionResponse) GetModifiedByUser() UserDetailsResponse`

GetModifiedByUser returns the ModifiedByUser field if non-nil, zero value otherwise.

### GetModifiedByUserOk

`func (o *ActionResponse) GetModifiedByUserOk() (*UserDetailsResponse, bool)`

GetModifiedByUserOk returns a tuple with the ModifiedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModifiedByUser

`func (o *ActionResponse) SetModifiedByUser(v UserDetailsResponse)`

SetModifiedByUser sets ModifiedByUser field to given value.

### HasModifiedByUser

`func (o *ActionResponse) HasModifiedByUser() bool`

HasModifiedByUser returns a boolean if a field has been set.

### GetNoteModifiedByUser

`func (o *ActionResponse) GetNoteModifiedByUser() UserDetailsResponse`

GetNoteModifiedByUser returns the NoteModifiedByUser field if non-nil, zero value otherwise.

### GetNoteModifiedByUserOk

`func (o *ActionResponse) GetNoteModifiedByUserOk() (*UserDetailsResponse, bool)`

GetNoteModifiedByUserOk returns a tuple with the NoteModifiedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNoteModifiedByUser

`func (o *ActionResponse) SetNoteModifiedByUser(v UserDetailsResponse)`

SetNoteModifiedByUser sets NoteModifiedByUser field to given value.

### HasNoteModifiedByUser

`func (o *ActionResponse) HasNoteModifiedByUser() bool`

HasNoteModifiedByUser returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


