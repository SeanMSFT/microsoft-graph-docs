
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Drives["{drive-id}"]
	.Request()
	.GetAsync();

```