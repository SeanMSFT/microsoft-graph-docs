
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = True;

await graphClient.ServicePrincipals["{id}"]
	.GetMemberObjects(securityEnabledOnly)
	.Request()
	.PostAsync()

```