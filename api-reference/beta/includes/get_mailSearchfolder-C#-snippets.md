
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolders = await graphClient.Me.MailFolders["AAMkAGVmMDEzN"]
	.Request()
	.GetAsync();

```