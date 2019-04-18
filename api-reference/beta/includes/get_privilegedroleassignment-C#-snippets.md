
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments["{id}"]
	.Request()
	.GetAsync();

```