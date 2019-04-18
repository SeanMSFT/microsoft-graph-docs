
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscriptions = await graphClient.Subscriptions["{id}"]
	.Request()
	.GetAsync();

```