
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var manager = await graphClient.Users["{id|userPrincipalName}"].Manager
	.Request()
	.GetAsync();

```