# CreateReportTemplateBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | Templatable report type (subset of ReportType that use templates) | 
**OrganisationId** | **string** | Organisation ID | 
**Name** | **string** | Report template display name | 

## Methods

### NewCreateReportTemplateBody

`func NewCreateReportTemplateBody(type_ string, organisationId string, name string, ) *CreateReportTemplateBody`

NewCreateReportTemplateBody instantiates a new CreateReportTemplateBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateReportTemplateBodyWithDefaults

`func NewCreateReportTemplateBodyWithDefaults() *CreateReportTemplateBody`

NewCreateReportTemplateBodyWithDefaults instantiates a new CreateReportTemplateBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CreateReportTemplateBody) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateReportTemplateBody) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateReportTemplateBody) SetType(v string)`

SetType sets Type field to given value.


### GetOrganisationId

`func (o *CreateReportTemplateBody) GetOrganisationId() string`

GetOrganisationId returns the OrganisationId field if non-nil, zero value otherwise.

### GetOrganisationIdOk

`func (o *CreateReportTemplateBody) GetOrganisationIdOk() (*string, bool)`

GetOrganisationIdOk returns a tuple with the OrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganisationId

`func (o *CreateReportTemplateBody) SetOrganisationId(v string)`

SetOrganisationId sets OrganisationId field to given value.


### GetName

`func (o *CreateReportTemplateBody) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateReportTemplateBody) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateReportTemplateBody) SetName(v string)`

SetName sets Name field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


