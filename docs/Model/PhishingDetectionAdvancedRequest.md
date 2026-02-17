# PhishingDetectionAdvancedRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input_string** | **string** | Input text string to detect phishing against | [optional] 
**model** | **string** | Optional: Specify which AI model to use.  Possible choices are Normal and Advanced.  Default is Advanced. | [optional] 
**custom_policy_id** | **string** | Apply a Custom Policy for Phishing Enforcement by providing the ID; to create a Custom Policy,  navigate to the Cloudmersive Management Portal and select Custom Policies.  Requires Managed Instance or Private Cloud | [optional] 
**provide_analysis_rationale** | **bool** | Optional: Set to true to include an analysis rationale in the response explaining why the content was or was not flagged.  Default is true. | [optional] 
**text_type** | **string** | Optional: Type of text being analyzed. Must be one of: \&quot;Text Message\&quot;, \&quot;User Message\&quot;, \&quot;Sales Lead\&quot;, \&quot;Email Message\&quot;, \&quot;Support Case\&quot;, \&quot;Other\&quot;. | [optional] 
**from_name** | **string** | Optional: Name of the sender | [optional] 
**to_name** | **string** | Optional: Name of the recipient | [optional] 
**from_phone_number** | **string** | Optional: Phone number of the sender | [optional] 
**to_phone_number** | **string** | Optional: Phone number of the recipient | [optional] 
**from_email_address** | **string** | Optional: Email address of the sender | [optional] 
**to_email_address** | **string** | Optional: Email address of the recipient | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


