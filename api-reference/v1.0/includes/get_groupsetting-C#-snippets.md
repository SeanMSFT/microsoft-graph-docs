
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettings = await graphClient.GroupSettings["{id}"]
	.Request()
	.GetAsync();

```