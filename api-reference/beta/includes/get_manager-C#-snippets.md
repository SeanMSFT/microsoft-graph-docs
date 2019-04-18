
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var manager = await graphClient.Contacts["{id}"].Manager
	.Request()
	.GetAsync();

```