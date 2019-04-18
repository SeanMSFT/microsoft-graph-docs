
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplates = await graphClient.DirectoryRoleTemplates["{id}"]
	.Request()
	.GetAsync();

```