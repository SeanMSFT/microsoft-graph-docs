
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["{id}"].Channels["{id}"].Messages["{id}"]
	.Request()
	.GetAsync();

```