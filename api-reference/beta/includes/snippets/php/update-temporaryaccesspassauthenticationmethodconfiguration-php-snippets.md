---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new AuthenticationMethodConfiguration();
$requestBody->set@odatatype('#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration');

$additionalData = [
		'isUsableOnce' => true,
];
$requestBody->setAdditionalData($additionalData);




$result = $graphServiceClient->policies()->authenticationMethodsPolicy()->authenticationMethodConfigurations()->byAuthenticationMethodConfigurationId('authenticationMethodConfiguration-id')->patch($requestBody);


```