# cloudmersive_phishing_api_client
Easily and directly scan and block phishing security threats in input.

[Cloudmersive Phishing API](https://cloudmersive.com/phishing-detection-api) provides advanced phishing detection capabilities.

- API version: v1
- Package version: 3.0.0


## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/cloudmersive/cloudmersive_phishing_api_client.git"
    }
  ],
  "require": {
    "cloudmersive/cloudmersive_phishing_api_client": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/cloudmersive_phishing_api_client/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## Documentation for API Endpoints

All URIs are relative to *https://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*PhishingDetectionApi* | [**phishingDetectEmailAdvancedPost**](docs/Api/PhishingDetectionApi.md#phishingdetectemailadvancedpost) | **POST** /phishing/detect/email/advanced | Perform advanced AI phishing detection and classification against input email.  Analyzes input email as well as embedded URLs with AI deep learning to detect phishing, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.
*PhishingDetectionApi* | [**phishingDetectFileAdvancedPost**](docs/Api/PhishingDetectionApi.md#phishingdetectfileadvancedpost) | **POST** /phishing/detect/file/advanced | Perform advanced AI phishing detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learning to detect phishing, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.
*PhishingDetectionApi* | [**phishingDetectFilePost**](docs/Api/PhishingDetectionApi.md#phishingdetectfilepost) | **POST** /phishing/detect/file | Perform AI phishing detection and classification on an input image or document (PDF or DOCX).  Analyzes input content as well as embedded URLs with AI deep learnign to detect phishing and other unsafe content.  Uses 100-125 API calls depending on model selected.
*PhishingDetectionApi* | [**phishingDetectTextStringAdvancedPost**](docs/Api/PhishingDetectionApi.md#phishingdetecttextstringadvancedpost) | **POST** /phishing/detect/text-string/advanced | Perform advanced AI phishing detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.


## Documentation For Models

 - [AdvancedEmailDetectionRequest](docs/Model/AdvancedEmailDetectionRequest.md)
 - [PhishingDetectionAdvancedRequest](docs/Model/PhishingDetectionAdvancedRequest.md)
 - [PhishingDetectionAdvancedResponse](docs/Model/PhishingDetectionAdvancedResponse.md)
 - [PhishingDetectionEmailAdvancedResponse](docs/Model/PhishingDetectionEmailAdvancedResponse.md)
 - [PhishingDetectionResponse](docs/Model/PhishingDetectionResponse.md)


## Documentation For Authorization


## Apikey

- **Type**: API key
- **API key parameter name**: Apikey
- **Location**: HTTP header


## Author




