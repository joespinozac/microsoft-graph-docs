---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



graphClient.Sites().BySiteId("site-id").Pages().ByPageId("sitePage-id").WebParts().ByWebPartId("webPart-id").GetPositionOfWebPart().Get(context.Background(), nil)


```