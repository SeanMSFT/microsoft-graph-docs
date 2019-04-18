
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alerts = await graphClient.Security.Alerts["{id}"]
	.Request()
	.GetAsync();

```