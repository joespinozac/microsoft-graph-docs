---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new Chart();
$additionalData = [
		'index' => 8,
];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->drives()->byDriveId('drive-id')->items()->byItemId('driveItem-id')->workbook()->worksheets()->byWorksheetId('workbookWorksheet-id')->charts()->byChartId('workbookChart-id')->post($requestBody);


```