# ScanDataWebPresenceRedirectResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Redirect ID | 
**Url** | **string** | URL | 
**StatusCode** | **int32** | HTTP status code | 
**TlsStatus** | **string** | Can be one of &#x60;http&#x60;, &#x60;https&#x60;, &#x60;http-risk&#x60;, &#x60;https-risk&#x60; | 

## Methods

### NewScanDataWebPresenceRedirectResponse

`func NewScanDataWebPresenceRedirectResponse(id string, url string, statusCode int32, tlsStatus string, ) *ScanDataWebPresenceRedirectResponse`

NewScanDataWebPresenceRedirectResponse instantiates a new ScanDataWebPresenceRedirectResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataWebPresenceRedirectResponseWithDefaults

`func NewScanDataWebPresenceRedirectResponseWithDefaults() *ScanDataWebPresenceRedirectResponse`

NewScanDataWebPresenceRedirectResponseWithDefaults instantiates a new ScanDataWebPresenceRedirectResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataWebPresenceRedirectResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataWebPresenceRedirectResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataWebPresenceRedirectResponse) SetId(v string)`

SetId sets Id field to given value.


### GetUrl

`func (o *ScanDataWebPresenceRedirectResponse) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ScanDataWebPresenceRedirectResponse) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ScanDataWebPresenceRedirectResponse) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetStatusCode

`func (o *ScanDataWebPresenceRedirectResponse) GetStatusCode() int32`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *ScanDataWebPresenceRedirectResponse) GetStatusCodeOk() (*int32, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *ScanDataWebPresenceRedirectResponse) SetStatusCode(v int32)`

SetStatusCode sets StatusCode field to given value.


### GetTlsStatus

`func (o *ScanDataWebPresenceRedirectResponse) GetTlsStatus() string`

GetTlsStatus returns the TlsStatus field if non-nil, zero value otherwise.

### GetTlsStatusOk

`func (o *ScanDataWebPresenceRedirectResponse) GetTlsStatusOk() (*string, bool)`

GetTlsStatusOk returns a tuple with the TlsStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTlsStatus

`func (o *ScanDataWebPresenceRedirectResponse) SetTlsStatus(v string)`

SetTlsStatus sets TlsStatus field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


