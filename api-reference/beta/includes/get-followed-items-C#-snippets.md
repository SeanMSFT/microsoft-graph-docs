
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Following
	.Request()
	.GetAsync();

```