
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts["{id}"]
	.Request()
	.GetAsync();

```