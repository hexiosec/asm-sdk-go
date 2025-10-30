# ScanDataRiskResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LinkId** | **string** | Link ID of Risk | 
**RiskNodeId** | **string** | Node ID of Risk | 
**Urn** | **string** | URN of Risk | 
**AssetType** | **string** | Type of Risk&#39;s parent | 
**AssetName** | **string** | Name of Risk&#39;s parent | 
**AssetNodeId** | **string** | Node ID of Risk&#39;s parent | 
**Name** | **string** | Name of Risk | 
**Description** | **string** | Description of Risk | 
**Remediation** | **string** | Remediation of Risk | 
**Severity** | **string** | Severity of Risk | 
**Category** | Pointer to **string** | Category of Risk | [optional] 
**Tags** | Pointer to **[]string** | Tags of Risk | [optional] 
**HasKnownExploit** | **bool** | Risk has a known exploit | 
**IsBrRisk** | **bool** | Risk may have backported security patches applied | 
**EpssScore** | Pointer to **float32** | Exploit Prediction Scoring System score of CVE, if risk isn&#39;t a CVE then this is omitted | [optional] 
**EpssPercentile** | Pointer to **float32** | Exploit Prediction Scoring System percentile of CVE, if risk isn&#39;t a CVE then this is omitted | [optional] 
**EpssModelVer** | Pointer to **string** | Exploit Prediction Scoring System model version used for CVE, if risk isn&#39;t a CVE then this is omitted | [optional] 
**EpssLastUpdate** | Pointer to **time.Time** | Exploit Prediction Scoring System last update for CVE, if risk isn&#39;t a CVE then this is omitted | [optional] 
**Created** | **time.Time** | Creation date of Risk | 
**LastSeen** | **time.Time** | Last seen data of Risk | 

## Methods

### NewScanDataRiskResponse

`func NewScanDataRiskResponse(linkId string, riskNodeId string, urn string, assetType string, assetName string, assetNodeId string, name string, description string, remediation string, severity string, hasKnownExploit bool, isBrRisk bool, created time.Time, lastSeen time.Time, ) *ScanDataRiskResponse`

NewScanDataRiskResponse instantiates a new ScanDataRiskResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataRiskResponseWithDefaults

`func NewScanDataRiskResponseWithDefaults() *ScanDataRiskResponse`

NewScanDataRiskResponseWithDefaults instantiates a new ScanDataRiskResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLinkId

`func (o *ScanDataRiskResponse) GetLinkId() string`

GetLinkId returns the LinkId field if non-nil, zero value otherwise.

### GetLinkIdOk

`func (o *ScanDataRiskResponse) GetLinkIdOk() (*string, bool)`

GetLinkIdOk returns a tuple with the LinkId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinkId

`func (o *ScanDataRiskResponse) SetLinkId(v string)`

SetLinkId sets LinkId field to given value.


### GetRiskNodeId

`func (o *ScanDataRiskResponse) GetRiskNodeId() string`

GetRiskNodeId returns the RiskNodeId field if non-nil, zero value otherwise.

### GetRiskNodeIdOk

`func (o *ScanDataRiskResponse) GetRiskNodeIdOk() (*string, bool)`

GetRiskNodeIdOk returns a tuple with the RiskNodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskNodeId

`func (o *ScanDataRiskResponse) SetRiskNodeId(v string)`

SetRiskNodeId sets RiskNodeId field to given value.


### GetUrn

`func (o *ScanDataRiskResponse) GetUrn() string`

GetUrn returns the Urn field if non-nil, zero value otherwise.

### GetUrnOk

`func (o *ScanDataRiskResponse) GetUrnOk() (*string, bool)`

GetUrnOk returns a tuple with the Urn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrn

`func (o *ScanDataRiskResponse) SetUrn(v string)`

SetUrn sets Urn field to given value.


### GetAssetType

`func (o *ScanDataRiskResponse) GetAssetType() string`

GetAssetType returns the AssetType field if non-nil, zero value otherwise.

### GetAssetTypeOk

`func (o *ScanDataRiskResponse) GetAssetTypeOk() (*string, bool)`

GetAssetTypeOk returns a tuple with the AssetType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetType

`func (o *ScanDataRiskResponse) SetAssetType(v string)`

SetAssetType sets AssetType field to given value.


### GetAssetName

`func (o *ScanDataRiskResponse) GetAssetName() string`

GetAssetName returns the AssetName field if non-nil, zero value otherwise.

### GetAssetNameOk

`func (o *ScanDataRiskResponse) GetAssetNameOk() (*string, bool)`

GetAssetNameOk returns a tuple with the AssetName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetName

`func (o *ScanDataRiskResponse) SetAssetName(v string)`

SetAssetName sets AssetName field to given value.


### GetAssetNodeId

`func (o *ScanDataRiskResponse) GetAssetNodeId() string`

GetAssetNodeId returns the AssetNodeId field if non-nil, zero value otherwise.

### GetAssetNodeIdOk

`func (o *ScanDataRiskResponse) GetAssetNodeIdOk() (*string, bool)`

GetAssetNodeIdOk returns a tuple with the AssetNodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetNodeId

`func (o *ScanDataRiskResponse) SetAssetNodeId(v string)`

SetAssetNodeId sets AssetNodeId field to given value.


### GetName

`func (o *ScanDataRiskResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanDataRiskResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanDataRiskResponse) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *ScanDataRiskResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ScanDataRiskResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ScanDataRiskResponse) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetRemediation

`func (o *ScanDataRiskResponse) GetRemediation() string`

GetRemediation returns the Remediation field if non-nil, zero value otherwise.

### GetRemediationOk

`func (o *ScanDataRiskResponse) GetRemediationOk() (*string, bool)`

GetRemediationOk returns a tuple with the Remediation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemediation

`func (o *ScanDataRiskResponse) SetRemediation(v string)`

SetRemediation sets Remediation field to given value.


### GetSeverity

`func (o *ScanDataRiskResponse) GetSeverity() string`

GetSeverity returns the Severity field if non-nil, zero value otherwise.

### GetSeverityOk

`func (o *ScanDataRiskResponse) GetSeverityOk() (*string, bool)`

GetSeverityOk returns a tuple with the Severity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeverity

`func (o *ScanDataRiskResponse) SetSeverity(v string)`

SetSeverity sets Severity field to given value.


### GetCategory

`func (o *ScanDataRiskResponse) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *ScanDataRiskResponse) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *ScanDataRiskResponse) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *ScanDataRiskResponse) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### GetTags

`func (o *ScanDataRiskResponse) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *ScanDataRiskResponse) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *ScanDataRiskResponse) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *ScanDataRiskResponse) HasTags() bool`

HasTags returns a boolean if a field has been set.

### GetHasKnownExploit

`func (o *ScanDataRiskResponse) GetHasKnownExploit() bool`

GetHasKnownExploit returns the HasKnownExploit field if non-nil, zero value otherwise.

### GetHasKnownExploitOk

`func (o *ScanDataRiskResponse) GetHasKnownExploitOk() (*bool, bool)`

GetHasKnownExploitOk returns a tuple with the HasKnownExploit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasKnownExploit

`func (o *ScanDataRiskResponse) SetHasKnownExploit(v bool)`

SetHasKnownExploit sets HasKnownExploit field to given value.


### GetIsBrRisk

`func (o *ScanDataRiskResponse) GetIsBrRisk() bool`

GetIsBrRisk returns the IsBrRisk field if non-nil, zero value otherwise.

### GetIsBrRiskOk

`func (o *ScanDataRiskResponse) GetIsBrRiskOk() (*bool, bool)`

GetIsBrRiskOk returns a tuple with the IsBrRisk field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsBrRisk

`func (o *ScanDataRiskResponse) SetIsBrRisk(v bool)`

SetIsBrRisk sets IsBrRisk field to given value.


### GetEpssScore

`func (o *ScanDataRiskResponse) GetEpssScore() float32`

GetEpssScore returns the EpssScore field if non-nil, zero value otherwise.

### GetEpssScoreOk

`func (o *ScanDataRiskResponse) GetEpssScoreOk() (*float32, bool)`

GetEpssScoreOk returns a tuple with the EpssScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpssScore

`func (o *ScanDataRiskResponse) SetEpssScore(v float32)`

SetEpssScore sets EpssScore field to given value.

### HasEpssScore

`func (o *ScanDataRiskResponse) HasEpssScore() bool`

HasEpssScore returns a boolean if a field has been set.

### GetEpssPercentile

`func (o *ScanDataRiskResponse) GetEpssPercentile() float32`

GetEpssPercentile returns the EpssPercentile field if non-nil, zero value otherwise.

### GetEpssPercentileOk

`func (o *ScanDataRiskResponse) GetEpssPercentileOk() (*float32, bool)`

GetEpssPercentileOk returns a tuple with the EpssPercentile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpssPercentile

`func (o *ScanDataRiskResponse) SetEpssPercentile(v float32)`

SetEpssPercentile sets EpssPercentile field to given value.

### HasEpssPercentile

`func (o *ScanDataRiskResponse) HasEpssPercentile() bool`

HasEpssPercentile returns a boolean if a field has been set.

### GetEpssModelVer

`func (o *ScanDataRiskResponse) GetEpssModelVer() string`

GetEpssModelVer returns the EpssModelVer field if non-nil, zero value otherwise.

### GetEpssModelVerOk

`func (o *ScanDataRiskResponse) GetEpssModelVerOk() (*string, bool)`

GetEpssModelVerOk returns a tuple with the EpssModelVer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpssModelVer

`func (o *ScanDataRiskResponse) SetEpssModelVer(v string)`

SetEpssModelVer sets EpssModelVer field to given value.

### HasEpssModelVer

`func (o *ScanDataRiskResponse) HasEpssModelVer() bool`

HasEpssModelVer returns a boolean if a field has been set.

### GetEpssLastUpdate

`func (o *ScanDataRiskResponse) GetEpssLastUpdate() time.Time`

GetEpssLastUpdate returns the EpssLastUpdate field if non-nil, zero value otherwise.

### GetEpssLastUpdateOk

`func (o *ScanDataRiskResponse) GetEpssLastUpdateOk() (*time.Time, bool)`

GetEpssLastUpdateOk returns a tuple with the EpssLastUpdate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpssLastUpdate

`func (o *ScanDataRiskResponse) SetEpssLastUpdate(v time.Time)`

SetEpssLastUpdate sets EpssLastUpdate field to given value.

### HasEpssLastUpdate

`func (o *ScanDataRiskResponse) HasEpssLastUpdate() bool`

HasEpssLastUpdate returns a boolean if a field has been set.

### GetCreated

`func (o *ScanDataRiskResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanDataRiskResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanDataRiskResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetLastSeen

`func (o *ScanDataRiskResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanDataRiskResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanDataRiskResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


