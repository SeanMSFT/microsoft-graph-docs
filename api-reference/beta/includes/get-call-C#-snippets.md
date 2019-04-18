
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calls = await graphClient.App.Calls["{id}"]
	.Request()
	.GetAsync();

```