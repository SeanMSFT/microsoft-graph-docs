
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoles = await graphClient.PrivilegedRoles["{id}"]
	.Request()
	.GetAsync();

```