
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts["{id}"]
	.Request()
	.GetAsync();

```