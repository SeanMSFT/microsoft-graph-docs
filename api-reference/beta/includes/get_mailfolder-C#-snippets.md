
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolders = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
	.Request()
	.GetAsync();

```