
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alerts = await graphClient.Security.Alerts["{alert_id}"]
	.Request()
	.GetAsync();

```