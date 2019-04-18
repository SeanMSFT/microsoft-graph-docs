
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = True;

await graphClient.Domains["contoso.com"]
	.ForceDelete(disableUserAccounts)
	.Request()
	.PostAsync()

```