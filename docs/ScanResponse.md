# ScanResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Scan ID | 
**Name** | **string** | Scan name | 
**ScanGroupId** | Pointer to **string** | Scan Group ID | [optional] 
**ScanGroupName** | Pointer to **string** | Scan Group name if requested | [optional] 
**Type** | [**ScanType**](ScanType.md) |  | 
**Enabled** | **bool** | Scan enabled | 
**Deleted** | **bool** | Scan deleted | 
**Created** | **time.Time** | Timestamp at which the entry was created | 
**CreatedBy** | **string** | User ID of the creator user | 
**Updated** | **time.Time** | Timestamp at which the entry was last updated | 
**Node** | Pointer to **map[string]interface{}** | Scan graph root node if requested | [optional] 
**Iteration** | Pointer to **map[string]interface{}** | Latest scan iteration state if requested | [optional] 
**CreatedByUser** | Pointer to [**UserDetailsResponse**](UserDetailsResponse.md) |  | [optional] 
**Monitor** | Pointer to **bool** | Scan has continuous monitor enabled | [optional] 
**MonitorSchedule** | Pointer to **string** | The frequency of the continuous scans | [optional] 
**MonitorNext** | Pointer to **time.Time** | The next time continuous monitoring will trigger a scan | [optional] 
**ShallowPageDepth** | Pointer to **float32** | Scan configuration | [optional] 
**DeepPageDepth** | Pointer to **float32** | Scan configuration | [optional] 
**DnsNamelist** | Pointer to **bool** | Scan configuration | [optional] 
**IgnoreIpNodes** | Pointer to **bool** | Scan configuration | [optional] 
**IncludeBrRisks** | **map[string]interface{}** | Config for backported resolvable risks | 
**InsightsGenerated** | Pointer to **time.Time** | Timestamp at which the insights were generated | [optional] 
**Insights** | Pointer to **map[string]interface{}** | Insights for Scan | [optional] 
**Seeds** | Pointer to **float32** | Number of seeds associated with scan | [optional] 
**Groups** | Pointer to [**[]Group**](Group.md) | Permission groups the user has for this scan if requested | [optional] 
**Roles** | Pointer to [**[]Role**](Role.md) | Permission roles the user has for this scan if requested | [optional] 
**OrganisationId** | Pointer to **string** | Organisation ID the scan belongs to if requested | [optional] 

## Methods

### NewScanResponse

`func NewScanResponse(id string, name string, type_ ScanType, enabled bool, deleted bool, created time.Time, createdBy string, updated time.Time, includeBrRisks map[string]interface{}, ) *ScanResponse`

NewScanResponse instantiates a new ScanResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanResponseWithDefaults

`func NewScanResponseWithDefaults() *ScanResponse`

NewScanResponseWithDefaults instantiates a new ScanResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ScanResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanResponse) SetName(v string)`

SetName sets Name field to given value.


### GetScanGroupId

`func (o *ScanResponse) GetScanGroupId() string`

GetScanGroupId returns the ScanGroupId field if non-nil, zero value otherwise.

### GetScanGroupIdOk

`func (o *ScanResponse) GetScanGroupIdOk() (*string, bool)`

GetScanGroupIdOk returns a tuple with the ScanGroupId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanGroupId

`func (o *ScanResponse) SetScanGroupId(v string)`

SetScanGroupId sets ScanGroupId field to given value.

### HasScanGroupId

`func (o *ScanResponse) HasScanGroupId() bool`

HasScanGroupId returns a boolean if a field has been set.

### GetScanGroupName

`func (o *ScanResponse) GetScanGroupName() string`

GetScanGroupName returns the ScanGroupName field if non-nil, zero value otherwise.

### GetScanGroupNameOk

`func (o *ScanResponse) GetScanGroupNameOk() (*string, bool)`

GetScanGroupNameOk returns a tuple with the ScanGroupName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanGroupName

`func (o *ScanResponse) SetScanGroupName(v string)`

SetScanGroupName sets ScanGroupName field to given value.

### HasScanGroupName

`func (o *ScanResponse) HasScanGroupName() bool`

HasScanGroupName returns a boolean if a field has been set.

### GetType

`func (o *ScanResponse) GetType() ScanType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ScanResponse) GetTypeOk() (*ScanType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ScanResponse) SetType(v ScanType)`

SetType sets Type field to given value.


### GetEnabled

`func (o *ScanResponse) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ScanResponse) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ScanResponse) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetDeleted

`func (o *ScanResponse) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *ScanResponse) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *ScanResponse) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.


### GetCreated

`func (o *ScanResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetCreatedBy

`func (o *ScanResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *ScanResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *ScanResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetUpdated

`func (o *ScanResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *ScanResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *ScanResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetNode

`func (o *ScanResponse) GetNode() map[string]interface{}`

GetNode returns the Node field if non-nil, zero value otherwise.

### GetNodeOk

`func (o *ScanResponse) GetNodeOk() (*map[string]interface{}, bool)`

GetNodeOk returns a tuple with the Node field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNode

`func (o *ScanResponse) SetNode(v map[string]interface{})`

SetNode sets Node field to given value.

### HasNode

`func (o *ScanResponse) HasNode() bool`

HasNode returns a boolean if a field has been set.

### GetIteration

`func (o *ScanResponse) GetIteration() map[string]interface{}`

GetIteration returns the Iteration field if non-nil, zero value otherwise.

### GetIterationOk

`func (o *ScanResponse) GetIterationOk() (*map[string]interface{}, bool)`

GetIterationOk returns a tuple with the Iteration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIteration

`func (o *ScanResponse) SetIteration(v map[string]interface{})`

SetIteration sets Iteration field to given value.

### HasIteration

`func (o *ScanResponse) HasIteration() bool`

HasIteration returns a boolean if a field has been set.

### GetCreatedByUser

`func (o *ScanResponse) GetCreatedByUser() UserDetailsResponse`

GetCreatedByUser returns the CreatedByUser field if non-nil, zero value otherwise.

### GetCreatedByUserOk

`func (o *ScanResponse) GetCreatedByUserOk() (*UserDetailsResponse, bool)`

GetCreatedByUserOk returns a tuple with the CreatedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedByUser

`func (o *ScanResponse) SetCreatedByUser(v UserDetailsResponse)`

SetCreatedByUser sets CreatedByUser field to given value.

### HasCreatedByUser

`func (o *ScanResponse) HasCreatedByUser() bool`

HasCreatedByUser returns a boolean if a field has been set.

### GetMonitor

`func (o *ScanResponse) GetMonitor() bool`

GetMonitor returns the Monitor field if non-nil, zero value otherwise.

### GetMonitorOk

`func (o *ScanResponse) GetMonitorOk() (*bool, bool)`

GetMonitorOk returns a tuple with the Monitor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitor

`func (o *ScanResponse) SetMonitor(v bool)`

SetMonitor sets Monitor field to given value.

### HasMonitor

`func (o *ScanResponse) HasMonitor() bool`

HasMonitor returns a boolean if a field has been set.

### GetMonitorSchedule

`func (o *ScanResponse) GetMonitorSchedule() string`

GetMonitorSchedule returns the MonitorSchedule field if non-nil, zero value otherwise.

### GetMonitorScheduleOk

`func (o *ScanResponse) GetMonitorScheduleOk() (*string, bool)`

GetMonitorScheduleOk returns a tuple with the MonitorSchedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorSchedule

`func (o *ScanResponse) SetMonitorSchedule(v string)`

SetMonitorSchedule sets MonitorSchedule field to given value.

### HasMonitorSchedule

`func (o *ScanResponse) HasMonitorSchedule() bool`

HasMonitorSchedule returns a boolean if a field has been set.

### GetMonitorNext

`func (o *ScanResponse) GetMonitorNext() time.Time`

GetMonitorNext returns the MonitorNext field if non-nil, zero value otherwise.

### GetMonitorNextOk

`func (o *ScanResponse) GetMonitorNextOk() (*time.Time, bool)`

GetMonitorNextOk returns a tuple with the MonitorNext field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorNext

`func (o *ScanResponse) SetMonitorNext(v time.Time)`

SetMonitorNext sets MonitorNext field to given value.

### HasMonitorNext

`func (o *ScanResponse) HasMonitorNext() bool`

HasMonitorNext returns a boolean if a field has been set.

### GetShallowPageDepth

`func (o *ScanResponse) GetShallowPageDepth() float32`

GetShallowPageDepth returns the ShallowPageDepth field if non-nil, zero value otherwise.

### GetShallowPageDepthOk

`func (o *ScanResponse) GetShallowPageDepthOk() (*float32, bool)`

GetShallowPageDepthOk returns a tuple with the ShallowPageDepth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShallowPageDepth

`func (o *ScanResponse) SetShallowPageDepth(v float32)`

SetShallowPageDepth sets ShallowPageDepth field to given value.

### HasShallowPageDepth

`func (o *ScanResponse) HasShallowPageDepth() bool`

HasShallowPageDepth returns a boolean if a field has been set.

### GetDeepPageDepth

`func (o *ScanResponse) GetDeepPageDepth() float32`

GetDeepPageDepth returns the DeepPageDepth field if non-nil, zero value otherwise.

### GetDeepPageDepthOk

`func (o *ScanResponse) GetDeepPageDepthOk() (*float32, bool)`

GetDeepPageDepthOk returns a tuple with the DeepPageDepth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeepPageDepth

`func (o *ScanResponse) SetDeepPageDepth(v float32)`

SetDeepPageDepth sets DeepPageDepth field to given value.

### HasDeepPageDepth

`func (o *ScanResponse) HasDeepPageDepth() bool`

HasDeepPageDepth returns a boolean if a field has been set.

### GetDnsNamelist

`func (o *ScanResponse) GetDnsNamelist() bool`

GetDnsNamelist returns the DnsNamelist field if non-nil, zero value otherwise.

### GetDnsNamelistOk

`func (o *ScanResponse) GetDnsNamelistOk() (*bool, bool)`

GetDnsNamelistOk returns a tuple with the DnsNamelist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDnsNamelist

`func (o *ScanResponse) SetDnsNamelist(v bool)`

SetDnsNamelist sets DnsNamelist field to given value.

### HasDnsNamelist

`func (o *ScanResponse) HasDnsNamelist() bool`

HasDnsNamelist returns a boolean if a field has been set.

### GetIgnoreIpNodes

`func (o *ScanResponse) GetIgnoreIpNodes() bool`

GetIgnoreIpNodes returns the IgnoreIpNodes field if non-nil, zero value otherwise.

### GetIgnoreIpNodesOk

`func (o *ScanResponse) GetIgnoreIpNodesOk() (*bool, bool)`

GetIgnoreIpNodesOk returns a tuple with the IgnoreIpNodes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIgnoreIpNodes

`func (o *ScanResponse) SetIgnoreIpNodes(v bool)`

SetIgnoreIpNodes sets IgnoreIpNodes field to given value.

### HasIgnoreIpNodes

`func (o *ScanResponse) HasIgnoreIpNodes() bool`

HasIgnoreIpNodes returns a boolean if a field has been set.

### GetIncludeBrRisks

`func (o *ScanResponse) GetIncludeBrRisks() map[string]interface{}`

GetIncludeBrRisks returns the IncludeBrRisks field if non-nil, zero value otherwise.

### GetIncludeBrRisksOk

`func (o *ScanResponse) GetIncludeBrRisksOk() (*map[string]interface{}, bool)`

GetIncludeBrRisksOk returns a tuple with the IncludeBrRisks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeBrRisks

`func (o *ScanResponse) SetIncludeBrRisks(v map[string]interface{})`

SetIncludeBrRisks sets IncludeBrRisks field to given value.


### GetInsightsGenerated

`func (o *ScanResponse) GetInsightsGenerated() time.Time`

GetInsightsGenerated returns the InsightsGenerated field if non-nil, zero value otherwise.

### GetInsightsGeneratedOk

`func (o *ScanResponse) GetInsightsGeneratedOk() (*time.Time, bool)`

GetInsightsGeneratedOk returns a tuple with the InsightsGenerated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInsightsGenerated

`func (o *ScanResponse) SetInsightsGenerated(v time.Time)`

SetInsightsGenerated sets InsightsGenerated field to given value.

### HasInsightsGenerated

`func (o *ScanResponse) HasInsightsGenerated() bool`

HasInsightsGenerated returns a boolean if a field has been set.

### GetInsights

`func (o *ScanResponse) GetInsights() map[string]interface{}`

GetInsights returns the Insights field if non-nil, zero value otherwise.

### GetInsightsOk

`func (o *ScanResponse) GetInsightsOk() (*map[string]interface{}, bool)`

GetInsightsOk returns a tuple with the Insights field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInsights

`func (o *ScanResponse) SetInsights(v map[string]interface{})`

SetInsights sets Insights field to given value.

### HasInsights

`func (o *ScanResponse) HasInsights() bool`

HasInsights returns a boolean if a field has been set.

### GetSeeds

`func (o *ScanResponse) GetSeeds() float32`

GetSeeds returns the Seeds field if non-nil, zero value otherwise.

### GetSeedsOk

`func (o *ScanResponse) GetSeedsOk() (*float32, bool)`

GetSeedsOk returns a tuple with the Seeds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeeds

`func (o *ScanResponse) SetSeeds(v float32)`

SetSeeds sets Seeds field to given value.

### HasSeeds

`func (o *ScanResponse) HasSeeds() bool`

HasSeeds returns a boolean if a field has been set.

### GetGroups

`func (o *ScanResponse) GetGroups() []Group`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *ScanResponse) GetGroupsOk() (*[]Group, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *ScanResponse) SetGroups(v []Group)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *ScanResponse) HasGroups() bool`

HasGroups returns a boolean if a field has been set.

### GetRoles

`func (o *ScanResponse) GetRoles() []Role`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *ScanResponse) GetRolesOk() (*[]Role, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *ScanResponse) SetRoles(v []Role)`

SetRoles sets Roles field to given value.

### HasRoles

`func (o *ScanResponse) HasRoles() bool`

HasRoles returns a boolean if a field has been set.

### GetOrganisationId

`func (o *ScanResponse) GetOrganisationId() string`

GetOrganisationId returns the OrganisationId field if non-nil, zero value otherwise.

### GetOrganisationIdOk

`func (o *ScanResponse) GetOrganisationIdOk() (*string, bool)`

GetOrganisationIdOk returns a tuple with the OrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganisationId

`func (o *ScanResponse) SetOrganisationId(v string)`

SetOrganisationId sets OrganisationId field to given value.

### HasOrganisationId

`func (o *ScanResponse) HasOrganisationId() bool`

HasOrganisationId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


