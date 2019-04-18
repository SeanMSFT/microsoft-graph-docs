
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObjects = await graphClient.DirectoryObjects["{id}"]
	.Request()
	.GetAsync();

```