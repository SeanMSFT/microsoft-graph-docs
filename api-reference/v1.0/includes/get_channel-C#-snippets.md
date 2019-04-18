
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{id}"].Channels["{id}"]
	.Request()
	.GetAsync();

```