
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var summary = await graphClient.PrivilegedRoles["{id}"].Summary
	.Request()
	.GetAsync();

```