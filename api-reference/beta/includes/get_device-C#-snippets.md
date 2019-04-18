
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices["{id}"]
	.Request()
	.GetAsync();

```