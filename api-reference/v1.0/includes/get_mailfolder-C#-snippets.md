
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolders = await graphClient.Me.MailFolders["{id}"]
	.Request()
	.GetAsync();

```