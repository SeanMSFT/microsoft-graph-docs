
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolders = await graphClient.Me.ContactFolders["{id}"]
	.Request()
	.GetAsync();

```