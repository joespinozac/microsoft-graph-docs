---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConversationMember
{
	OdataType = "#microsoft.graph.aadUserConversationMember",
	Roles = new List<String>
	{
	},
	AdditionalData = new Dictionary<string, object>
	{
		{
			"user@odata.bind" , "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
		},
	},
};
var result = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members.PostAsync(requestBody);


```