
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoles = await graphClient.DirectoryRoles["{id}"]
	.Request()
	.GetAsync();

```