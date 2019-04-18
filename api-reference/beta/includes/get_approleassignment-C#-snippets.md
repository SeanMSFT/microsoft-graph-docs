
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.AppRoleAssignments["{id}"]
	.Request()
	.GetAsync();

```