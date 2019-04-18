
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebooks = await graphClient.Me.Onenote.Notebooks["{id}"]
	.Request()
	.GetAsync();

```