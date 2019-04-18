
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Education.Users["{user-id}"]
	.Request()
	.GetAsync();

```