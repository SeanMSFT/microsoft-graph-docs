
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Teams["{id}"].Channels["{id}"].Messages["{id}"].Replies["{id}"]
	.Request()
	.GetAsync();

```