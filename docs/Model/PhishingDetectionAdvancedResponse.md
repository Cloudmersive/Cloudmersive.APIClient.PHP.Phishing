# PhishingDetectionAdvancedResponse

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**clean_result** | **bool** | True if the result is not phishing (clean), and false otherwise | [optional] 
**contains_phishing** | **bool** | True if the input text contains a phishing attempt, false otherwise | [optional] 
**contains_unsolicited_sales** | **bool** | True if the input text contains unsolicited sales, false otherwise | [optional] 
**contains_promotional_content** | **bool** | True if the input text contains promotional content, false otherwise | [optional] 
**contains_web_urls** | **bool** | True if the input text contains web URLs, including homoglyph URLs and spaced-out URL workarounds | [optional] 
**contains_phone_numbers** | **bool** | True if the input text contains phone numbers, including homoglyph digits and spaced-out or spelled-out workarounds | [optional] 
**contains_email_addresses** | **bool** | True if the input text contains email addresses, including homoglyph characters and obfuscated workarounds | [optional] 
**confidence_level** | **double** | Confidence level between 0.0 and 1.0 where values over 0.9 indicate high confidence | [optional] 
**analysis_rationale** | **string** | Rationale for why the conclusion was formed | [optional] 
**unsafe_urls** | [**\Swagger\Client\Model\UnsafeUrlResult[]**](UnsafeUrlResult.md) | URLs detected in the input text that were analyzed and found to be unsafe. Only populated when ProvideUrlAnalysis is true and URLs are detected. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


