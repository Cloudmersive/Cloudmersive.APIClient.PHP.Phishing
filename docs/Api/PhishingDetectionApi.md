# Swagger\Client\PhishingDetectionApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**phishingDetectEmailAdvancedPost**](PhishingDetectionApi.md#phishingDetectEmailAdvancedPost) | **POST** /phishing/detect/email/advanced | Perform advanced AI phishing detection and classification against input email.  Analyzes input email as well as embedded URLs with AI deep learning to detect phishing, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.
[**phishingDetectFileAdvancedPost**](PhishingDetectionApi.md#phishingDetectFileAdvancedPost) | **POST** /phishing/detect/file/advanced | Perform advanced AI phishing detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learning to detect phishing, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.
[**phishingDetectFilePost**](PhishingDetectionApi.md#phishingDetectFilePost) | **POST** /phishing/detect/file | Perform AI phishing detection and classification on an input image or document (PDF or DOCX).  Analyzes input content as well as embedded URLs with AI deep learnign to detect phishing and other unsafe content.  Uses 100-125 API calls depending on model selected.
[**phishingDetectTextStringAdvancedPost**](PhishingDetectionApi.md#phishingDetectTextStringAdvancedPost) | **POST** /phishing/detect/text-string/advanced | Perform advanced AI phishing detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.


# **phishingDetectEmailAdvancedPost**
> \Swagger\Client\Model\PhishingDetectionEmailAdvancedResponse phishingDetectEmailAdvancedPost($body)

Perform advanced AI phishing detection and classification against input email.  Analyzes input email as well as embedded URLs with AI deep learning to detect phishing, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PhishingDetectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\AdvancedEmailDetectionRequest(); // \Swagger\Client\Model\AdvancedEmailDetectionRequest | Phishing detection request

try {
    $result = $apiInstance->phishingDetectEmailAdvancedPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PhishingDetectionApi->phishingDetectEmailAdvancedPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\AdvancedEmailDetectionRequest**](../Model/AdvancedEmailDetectionRequest.md)| Phishing detection request | [optional]

### Return type

[**\Swagger\Client\Model\PhishingDetectionEmailAdvancedResponse**](../Model/PhishingDetectionEmailAdvancedResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **phishingDetectFileAdvancedPost**
> \Swagger\Client\Model\PhishingDetectionAdvancedResponse phishingDetectFileAdvancedPost($model, $input_file)

Perform advanced AI phishing detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learning to detect phishing, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PhishingDetectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$model = "Advanced"; // string | 
$input_file = "/path/to/file.txt"; // \SplFileObject | 

try {
    $result = $apiInstance->phishingDetectFileAdvancedPost($model, $input_file);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PhishingDetectionApi->phishingDetectFileAdvancedPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model** | **string**|  | [optional] [default to Advanced]
 **input_file** | **\SplFileObject**|  | [optional]

### Return type

[**\Swagger\Client\Model\PhishingDetectionAdvancedResponse**](../Model/PhishingDetectionAdvancedResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **phishingDetectFilePost**
> \Swagger\Client\Model\PhishingDetectionResponse phishingDetectFilePost($model, $input_file)

Perform AI phishing detection and classification on an input image or document (PDF or DOCX).  Analyzes input content as well as embedded URLs with AI deep learnign to detect phishing and other unsafe content.  Uses 100-125 API calls depending on model selected.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PhishingDetectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$model = "Advanced"; // string | Model to use; default setting is Advanced
$input_file = "/path/to/file.txt"; // \SplFileObject | 

try {
    $result = $apiInstance->phishingDetectFilePost($model, $input_file);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PhishingDetectionApi->phishingDetectFilePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model** | **string**| Model to use; default setting is Advanced | [optional] [default to Advanced]
 **input_file** | **\SplFileObject**|  | [optional]

### Return type

[**\Swagger\Client\Model\PhishingDetectionResponse**](../Model/PhishingDetectionResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **phishingDetectTextStringAdvancedPost**
> \Swagger\Client\Model\PhishingDetectionAdvancedResponse phishingDetectTextStringAdvancedPost($body)

Perform advanced AI phishing detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PhishingDetectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\PhishingDetectionAdvancedRequest(); // \Swagger\Client\Model\PhishingDetectionAdvancedRequest | Phishing detection request

try {
    $result = $apiInstance->phishingDetectTextStringAdvancedPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PhishingDetectionApi->phishingDetectTextStringAdvancedPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\PhishingDetectionAdvancedRequest**](../Model/PhishingDetectionAdvancedRequest.md)| Phishing detection request | [optional]

### Return type

[**\Swagger\Client\Model\PhishingDetectionAdvancedResponse**](../Model/PhishingDetectionAdvancedResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

