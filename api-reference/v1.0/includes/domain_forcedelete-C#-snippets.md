
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = True;

await graphClient.Domains["{id}"]
	.ForceDelete(disableUserAccounts)
	.Request()
	.PostAsync()

```