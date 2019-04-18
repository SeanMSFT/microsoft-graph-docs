
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users["{user-id}"]
	.Request()
	.GetAsync();

```