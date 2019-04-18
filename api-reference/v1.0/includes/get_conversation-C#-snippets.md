
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversations = await graphClient.Groups["{id}"].Conversations["{id}"]
	.Request()
	.GetAsync();

```