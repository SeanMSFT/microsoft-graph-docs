
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AppRoleAssignments["{id}"]
	.Request()
	.DeleteAsync();

```