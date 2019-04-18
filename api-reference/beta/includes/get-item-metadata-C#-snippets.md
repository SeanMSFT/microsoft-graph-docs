
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var root = await graphClient.Me.Drive.Root
	.Request()
	.GetAsync();

```