
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.PrivilegedRoles["{id}"].Settings
	.Request()
	.GetAsync();

```