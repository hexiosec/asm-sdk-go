# UpdateMarketingPreferencesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductMarketing** | Pointer to **bool** | Subscribe or unsubscribe the user from product marketing emails | [optional] 
**VendorMarketing** | Pointer to **bool** | Subscribe or unsubscribe the user from vendor marketing emails | [optional] 

## Methods

### NewUpdateMarketingPreferencesRequest

`func NewUpdateMarketingPreferencesRequest() *UpdateMarketingPreferencesRequest`

NewUpdateMarketingPreferencesRequest instantiates a new UpdateMarketingPreferencesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateMarketingPreferencesRequestWithDefaults

`func NewUpdateMarketingPreferencesRequestWithDefaults() *UpdateMarketingPreferencesRequest`

NewUpdateMarketingPreferencesRequestWithDefaults instantiates a new UpdateMarketingPreferencesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProductMarketing

`func (o *UpdateMarketingPreferencesRequest) GetProductMarketing() bool`

GetProductMarketing returns the ProductMarketing field if non-nil, zero value otherwise.

### GetProductMarketingOk

`func (o *UpdateMarketingPreferencesRequest) GetProductMarketingOk() (*bool, bool)`

GetProductMarketingOk returns a tuple with the ProductMarketing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductMarketing

`func (o *UpdateMarketingPreferencesRequest) SetProductMarketing(v bool)`

SetProductMarketing sets ProductMarketing field to given value.

### HasProductMarketing

`func (o *UpdateMarketingPreferencesRequest) HasProductMarketing() bool`

HasProductMarketing returns a boolean if a field has been set.

### GetVendorMarketing

`func (o *UpdateMarketingPreferencesRequest) GetVendorMarketing() bool`

GetVendorMarketing returns the VendorMarketing field if non-nil, zero value otherwise.

### GetVendorMarketingOk

`func (o *UpdateMarketingPreferencesRequest) GetVendorMarketingOk() (*bool, bool)`

GetVendorMarketingOk returns a tuple with the VendorMarketing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVendorMarketing

`func (o *UpdateMarketingPreferencesRequest) SetVendorMarketing(v bool)`

SetVendorMarketing sets VendorMarketing field to given value.

### HasVendorMarketing

`func (o *UpdateMarketingPreferencesRequest) HasVendorMarketing() bool`

HasVendorMarketing returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


