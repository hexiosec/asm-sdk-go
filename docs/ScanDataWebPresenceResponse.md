# ScanDataWebPresenceResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | URL ID | 
**Url** | **string** | URL | 
**Domain** | **string** | Domain | 
**ScreenshotId** | Pointer to **string** | Screenshot ID | [optional] 
**HttpServer** | Pointer to **string** | HTTP web server details | [optional] 
**StatusCode** | **int32** | HTTP status code | 
**PageTitle** | Pointer to **string** | Page title | [optional] 
**TlsStatus** | **string** | Can be one of &#x60;http&#x60;, &#x60;https&#x60;, &#x60;http-risk&#x60;, &#x60;https-risk&#x60; | 
**ContentType** | Pointer to **string** | Content type | [optional] 
**FormInput** | **bool** | Whether the web page at the URL contains a form input | 
**Components** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Components | 
**Redirects** | [**[]ScanDataWebPresenceRedirectResponse**](ScanDataWebPresenceRedirectResponse.md) | Redirects | 
**Created** | **time.Time** | URL creation date | 
**LastSeen** | **time.Time** | URL last seen date | 

## Methods

### NewScanDataWebPresenceResponse

`func NewScanDataWebPresenceResponse(id string, url string, domain string, statusCode int32, tlsStatus string, formInput bool, components []ScanDataNodeResponse, redirects []ScanDataWebPresenceRedirectResponse, created time.Time, lastSeen time.Time, ) *ScanDataWebPresenceResponse`

NewScanDataWebPresenceResponse instantiates a new ScanDataWebPresenceResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataWebPresenceResponseWithDefaults

`func NewScanDataWebPresenceResponseWithDefaults() *ScanDataWebPresenceResponse`

NewScanDataWebPresenceResponseWithDefaults instantiates a new ScanDataWebPresenceResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataWebPresenceResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataWebPresenceResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataWebPresenceResponse) SetId(v string)`

SetId sets Id field to given value.


### GetUrl

`func (o *ScanDataWebPresenceResponse) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ScanDataWebPresenceResponse) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ScanDataWebPresenceResponse) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetDomain

`func (o *ScanDataWebPresenceResponse) GetDomain() string`

GetDomain returns the Domain field if non-nil, zero value otherwise.

### GetDomainOk

`func (o *ScanDataWebPresenceResponse) GetDomainOk() (*string, bool)`

GetDomainOk returns a tuple with the Domain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomain

`func (o *ScanDataWebPresenceResponse) SetDomain(v string)`

SetDomain sets Domain field to given value.


### GetScreenshotId

`func (o *ScanDataWebPresenceResponse) GetScreenshotId() string`

GetScreenshotId returns the ScreenshotId field if non-nil, zero value otherwise.

### GetScreenshotIdOk

`func (o *ScanDataWebPresenceResponse) GetScreenshotIdOk() (*string, bool)`

GetScreenshotIdOk returns a tuple with the ScreenshotId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScreenshotId

`func (o *ScanDataWebPresenceResponse) SetScreenshotId(v string)`

SetScreenshotId sets ScreenshotId field to given value.

### HasScreenshotId

`func (o *ScanDataWebPresenceResponse) HasScreenshotId() bool`

HasScreenshotId returns a boolean if a field has been set.

### GetHttpServer

`func (o *ScanDataWebPresenceResponse) GetHttpServer() string`

GetHttpServer returns the HttpServer field if non-nil, zero value otherwise.

### GetHttpServerOk

`func (o *ScanDataWebPresenceResponse) GetHttpServerOk() (*string, bool)`

GetHttpServerOk returns a tuple with the HttpServer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpServer

`func (o *ScanDataWebPresenceResponse) SetHttpServer(v string)`

SetHttpServer sets HttpServer field to given value.

### HasHttpServer

`func (o *ScanDataWebPresenceResponse) HasHttpServer() bool`

HasHttpServer returns a boolean if a field has been set.

### GetStatusCode

`func (o *ScanDataWebPresenceResponse) GetStatusCode() int32`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *ScanDataWebPresenceResponse) GetStatusCodeOk() (*int32, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *ScanDataWebPresenceResponse) SetStatusCode(v int32)`

SetStatusCode sets StatusCode field to given value.


### GetPageTitle

`func (o *ScanDataWebPresenceResponse) GetPageTitle() string`

GetPageTitle returns the PageTitle field if non-nil, zero value otherwise.

### GetPageTitleOk

`func (o *ScanDataWebPresenceResponse) GetPageTitleOk() (*string, bool)`

GetPageTitleOk returns a tuple with the PageTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageTitle

`func (o *ScanDataWebPresenceResponse) SetPageTitle(v string)`

SetPageTitle sets PageTitle field to given value.

### HasPageTitle

`func (o *ScanDataWebPresenceResponse) HasPageTitle() bool`

HasPageTitle returns a boolean if a field has been set.

### GetTlsStatus

`func (o *ScanDataWebPresenceResponse) GetTlsStatus() string`

GetTlsStatus returns the TlsStatus field if non-nil, zero value otherwise.

### GetTlsStatusOk

`func (o *ScanDataWebPresenceResponse) GetTlsStatusOk() (*string, bool)`

GetTlsStatusOk returns a tuple with the TlsStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTlsStatus

`func (o *ScanDataWebPresenceResponse) SetTlsStatus(v string)`

SetTlsStatus sets TlsStatus field to given value.


### GetContentType

`func (o *ScanDataWebPresenceResponse) GetContentType() string`

GetContentType returns the ContentType field if non-nil, zero value otherwise.

### GetContentTypeOk

`func (o *ScanDataWebPresenceResponse) GetContentTypeOk() (*string, bool)`

GetContentTypeOk returns a tuple with the ContentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentType

`func (o *ScanDataWebPresenceResponse) SetContentType(v string)`

SetContentType sets ContentType field to given value.

### HasContentType

`func (o *ScanDataWebPresenceResponse) HasContentType() bool`

HasContentType returns a boolean if a field has been set.

### GetFormInput

`func (o *ScanDataWebPresenceResponse) GetFormInput() bool`

GetFormInput returns the FormInput field if non-nil, zero value otherwise.

### GetFormInputOk

`func (o *ScanDataWebPresenceResponse) GetFormInputOk() (*bool, bool)`

GetFormInputOk returns a tuple with the FormInput field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormInput

`func (o *ScanDataWebPresenceResponse) SetFormInput(v bool)`

SetFormInput sets FormInput field to given value.


### GetComponents

`func (o *ScanDataWebPresenceResponse) GetComponents() []ScanDataNodeResponse`

GetComponents returns the Components field if non-nil, zero value otherwise.

### GetComponentsOk

`func (o *ScanDataWebPresenceResponse) GetComponentsOk() (*[]ScanDataNodeResponse, bool)`

GetComponentsOk returns a tuple with the Components field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComponents

`func (o *ScanDataWebPresenceResponse) SetComponents(v []ScanDataNodeResponse)`

SetComponents sets Components field to given value.


### GetRedirects

`func (o *ScanDataWebPresenceResponse) GetRedirects() []ScanDataWebPresenceRedirectResponse`

GetRedirects returns the Redirects field if non-nil, zero value otherwise.

### GetRedirectsOk

`func (o *ScanDataWebPresenceResponse) GetRedirectsOk() (*[]ScanDataWebPresenceRedirectResponse, bool)`

GetRedirectsOk returns a tuple with the Redirects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirects

`func (o *ScanDataWebPresenceResponse) SetRedirects(v []ScanDataWebPresenceRedirectResponse)`

SetRedirects sets Redirects field to given value.


### GetCreated

`func (o *ScanDataWebPresenceResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanDataWebPresenceResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanDataWebPresenceResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetLastSeen

`func (o *ScanDataWebPresenceResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanDataWebPresenceResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanDataWebPresenceResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


