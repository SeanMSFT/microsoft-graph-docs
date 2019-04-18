
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var photo = await graphClient.Users["{id|userPrincipalName}"].Photo
	.Request()
	.GetAsync();

```