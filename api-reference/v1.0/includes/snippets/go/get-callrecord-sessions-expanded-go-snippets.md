---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphconfig "github.com/microsoftgraph/msgraph-sdk-go/communications"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestParameters := &graphconfig.CommunicationsCallRecordItemSessionsRequestBuilderGetQueryParameters{
	Expand: [] string {"segments"},
}
configuration := &graphconfig.CommunicationsCallRecordItemSessionsRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Communications().CallRecords().ByCallRecordId("callRecord-id").Sessions().Get(context.Background(), configuration)


```