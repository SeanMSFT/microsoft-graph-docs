
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = True;

await graphClient.ServicePrincipals["{id}"]
	.GetMemberGroups(securityEnabledOnly)
	.Request()
	.PostAsync()

```