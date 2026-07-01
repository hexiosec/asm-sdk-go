# CreateScanRequestIncludeBrRisks

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UrnComponentApplicationApache** | **bool** | Include backported resolvable risks for Apache | 
**UrnComponentApplicationOpenssl** | Pointer to **bool** | Include backported resolvable risks for OpenSSL | [optional] 

## Methods

### NewCreateScanRequestIncludeBrRisks

`func NewCreateScanRequestIncludeBrRisks(urnComponentApplicationApache bool, ) *CreateScanRequestIncludeBrRisks`

NewCreateScanRequestIncludeBrRisks instantiates a new CreateScanRequestIncludeBrRisks object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateScanRequestIncludeBrRisksWithDefaults

`func NewCreateScanRequestIncludeBrRisksWithDefaults() *CreateScanRequestIncludeBrRisks`

NewCreateScanRequestIncludeBrRisksWithDefaults instantiates a new CreateScanRequestIncludeBrRisks object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrnComponentApplicationApache

`func (o *CreateScanRequestIncludeBrRisks) GetUrnComponentApplicationApache() bool`

GetUrnComponentApplicationApache returns the UrnComponentApplicationApache field if non-nil, zero value otherwise.

### GetUrnComponentApplicationApacheOk

`func (o *CreateScanRequestIncludeBrRisks) GetUrnComponentApplicationApacheOk() (*bool, bool)`

GetUrnComponentApplicationApacheOk returns a tuple with the UrnComponentApplicationApache field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrnComponentApplicationApache

`func (o *CreateScanRequestIncludeBrRisks) SetUrnComponentApplicationApache(v bool)`

SetUrnComponentApplicationApache sets UrnComponentApplicationApache field to given value.


### GetUrnComponentApplicationOpenssl

`func (o *CreateScanRequestIncludeBrRisks) GetUrnComponentApplicationOpenssl() bool`

GetUrnComponentApplicationOpenssl returns the UrnComponentApplicationOpenssl field if non-nil, zero value otherwise.

### GetUrnComponentApplicationOpensslOk

`func (o *CreateScanRequestIncludeBrRisks) GetUrnComponentApplicationOpensslOk() (*bool, bool)`

GetUrnComponentApplicationOpensslOk returns a tuple with the UrnComponentApplicationOpenssl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrnComponentApplicationOpenssl

`func (o *CreateScanRequestIncludeBrRisks) SetUrnComponentApplicationOpenssl(v bool)`

SetUrnComponentApplicationOpenssl sets UrnComponentApplicationOpenssl field to given value.

### HasUrnComponentApplicationOpenssl

`func (o *CreateScanRequestIncludeBrRisks) HasUrnComponentApplicationOpenssl() bool`

HasUrnComponentApplicationOpenssl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


