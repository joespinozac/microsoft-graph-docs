---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/Security/MicrosoftGraphSecurityRunHuntingQuery"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewRunHuntingQueryPostRequestBody()
query := "DeviceProcessEvents | where InitiatingProcessFileName =~ \"powershell.exe\" | project Timestamp, FileName, InitiatingProcessFileName | order by Timestamp desc | limit 2"
requestBody.SetQuery(&query) 

result, err := graphClient.Security().MicrosoftGraphSecurityRunHuntingQuery().Post(context.Background(), requestBody, nil)


```