---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphconfig "github.com/microsoftgraph/msgraph-beta-sdk-go/print"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestParameters := &graphconfig.PrintPrinterItemJobItemRequestBuilderGetQueryParameters{
	Expand: [] string {"tasks"},
}
configuration := &graphconfig.PrintPrinterItemJobItemRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Print().Printers().ByPrinterId("printer-id").Jobs().ByJobId("printJob-id").Get(context.Background(), configuration)


```