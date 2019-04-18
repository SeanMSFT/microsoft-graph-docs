
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deletedItems = await graphClient.Directory.DeletedItems["{object-id}"]
	.Request()
	.GetAsync();

```