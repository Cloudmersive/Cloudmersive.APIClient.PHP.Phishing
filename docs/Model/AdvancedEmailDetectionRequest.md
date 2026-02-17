# AdvancedEmailDetectionRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_email_address** | **string** | Email address of the sender | [optional] 
**to_email_address** | **string** | Email address of the recipient | [optional] 
**subject** | **string** | Subject of the email | [optional] 
**html_body** | **string** | Body of the email in HTML, or text | [optional] 
**allow_low_reputation_senders** | **bool** | Allow email from low reputation senders and domains | [optional] 
**allow_sanctioned** | **bool** | True to allow sanctioned countries and certain known sanctioned entities, false otherwise (default) | [optional] 
**custom_policy_id** | **string** | Apply a Custom Policy for Phishing Enforcement by providing the ID; to create a Custom Policy,  navigate to the Cloudmersive Management Portal and select Custom Policies.  Requires Managed Instance or Private Cloud | [optional] 
**input_email_file** | **string** | Optional: Input email file bytes (EML, PDF, etc.).  If not provided, HtmlBody will be used instead. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


