
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var special = await graphClient.Me.Drive.Special["{name}"]
	.Request()
	.GetAsync();

```