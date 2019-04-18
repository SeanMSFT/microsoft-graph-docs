
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Education.Users["13012"]
	.Request()
	.GetAsync();

```