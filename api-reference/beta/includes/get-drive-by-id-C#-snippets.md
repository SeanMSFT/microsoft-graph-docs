
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Drives["{driveId}"]
	.Request()
	.GetAsync();

```