
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicators = await graphClient.Security.TiIndicators["{id}"]
	.Request()
	.GetAsync();

```