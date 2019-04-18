
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscriptions = await graphClient.Me.Drive.Root.Subscriptions["socketIo"]
	.Request()
	.GetAsync();

```