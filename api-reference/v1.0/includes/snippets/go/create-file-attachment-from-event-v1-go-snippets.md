---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/models"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewAttachment()
name := "menu.txt"
requestBody.SetName(&name) 
additionalData := map[string]interface{}{
	"contentBytes" : "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk=", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Me().Events().ByEventId("event-id").Attachments().Post(context.Background(), requestBody, nil)


```