
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeetings = await graphClient.App.OnlineMeetings["{id}"]
	.Request()
	.GetAsync();

```