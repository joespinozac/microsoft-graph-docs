---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Models.Security.EdiscoveryNoncustodialDataSource
{
	DataSource = new Microsoft.Graph.Models.Security.DataSource
	{
		OdataType = "microsoft.graph.security.siteSource",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"site" , new 
				{
					WebUrl = "https://m365x809305.sharepoint.com/sites/Design-topsecret",
				}
			},
		},
	},
};
var result = await graphClient.Security.Cases.EdiscoveryCases["{ediscoveryCase-id}"].NoncustodialDataSources.PostAsync(requestBody);


```