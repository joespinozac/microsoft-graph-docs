---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewGroup()
description := "Group with designated owner and members"
requestBody.SetDescription(&description) 
displayName := "Operations group"
requestBody.SetDisplayName(&displayName) 
groupTypes := []string {

}
requestBody.SetGroupTypes(groupTypes)
mailEnabled := false
requestBody.SetMailEnabled(&mailEnabled) 
mailNickname := "operations2019"
requestBody.SetMailNickname(&mailNickname) 
securityEnabled := true
requestBody.SetSecurityEnabled(&securityEnabled) 
additionalData := map[string]interface{}{
	odataBind := []string {
		"https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2",

	}
	odataBind := []string {
		"https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
		"https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14",

	}
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Groups().Post(context.Background(), requestBody, nil)


```