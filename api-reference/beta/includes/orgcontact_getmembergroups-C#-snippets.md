
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = True;

await graphClient.Contacts["{id}"]
	.GetMemberGroups(securityEnabledOnly)
	.Request()
	.PostAsync()

```