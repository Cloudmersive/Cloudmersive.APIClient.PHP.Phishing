# PhishingDetectionAdvancedRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input_string** | **string** | Input text string to detect phishing against | [optional] 
**text_type** | **string** | Optional: Type of text being analyzed. Must be one of: \&quot;TextMessage\&quot;, \&quot;UserMessage\&quot;, \&quot;SalesLead\&quot;, \&quot;EmailMessage\&quot;, \&quot;SupportCase\&quot;, \&quot;AppMessage\&quot;, \&quot;Other\&quot;. | [optional] 
**model** | **string** | Optional: Specify which AI model to use.  Possible choices are Normal and Advanced.  Default is Advanced. | [optional] 
**allow_unsolicited_sales** | **bool** | Optional: True if unsolicited sales should be allowed, false otherwise. Defaults to true. | [optional] 
**allow_promotional_content** | **bool** | Optional: True if promotional content should be allowed, false otherwise. Defaults to true. | [optional] 
**allow_web_urls** | **bool** | Optional: True if web URLs should be allowed in the input text, false otherwise. Defaults to true. When false, input containing URLs (including homoglyph URLs and spaced-out URLs) will be flagged as not clean. | [optional] 
**allow_phone_numbers** | **bool** | Optional: True if phone numbers should be allowed in the input text, false otherwise. Defaults to true. When false, input containing phone numbers (including homoglyph digits and spaced-out or spelled-out workarounds) will be flagged as not clean. | [optional] 
**allow_email_addresses** | **bool** | Optional: True if email addresses should be allowed in the input text, false otherwise. Defaults to true. When false, input containing email addresses (including homoglyph characters and obfuscated workarounds like \&quot;danny at somedomaine [DOT] com\&quot;) will be flagged as not clean. | [optional] 
**provide_url_analysis** | **bool** | Optional: True to perform deep URL analysis on any URLs detected in the text. When enabled, if the initial AI scan detects URLs, a second AI call enumerates them and each URL is individually analyzed for phishing. Defaults to true. | [optional] 
**custom_policy_id** | **string** | Apply a Custom Policy for Phishing Enforcement by providing the ID; to create a Custom Policy,  navigate to the Cloudmersive Management Portal and select Custom Policies.  Requires Managed Instance or Private Cloud | [optional] 
**provide_analysis_rationale** | **bool** | Optional: Set to true to include an analysis rationale in the response explaining why the content was or was not flagged.  Default is true. | [optional] 
**from_name** | **string** | Optional: Name of the sender | [optional] 
**to_name** | **string** | Optional: Name of the recipient | [optional] 
**from_phone_number** | **string** | Optional: Phone number of the sender | [optional] 
**to_phone_number** | **string** | Optional: Phone number of the recipient | [optional] 
**from_email_address** | **string** | Optional: Email address of the sender | [optional] 
**to_email_address** | **string** | Optional: Email address of the recipient | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


