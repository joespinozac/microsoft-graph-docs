---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphconfig "github.com/microsoftgraph/msgraph-sdk-go/users"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestFilter := "startsWith(subject,'All')"

requestParameters := &graphconfig.ItemCalendarEventsRequestBuilderGetQueryParameters{
	Filter: &requestFilter,
}
configuration := &graphconfig.ItemCalendarEventsRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Me().Calendar().Events().Get(context.Background(), configuration)


```