
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = True;

await graphClient.Me
	.GetMemberGroups(securityEnabledOnly)
	.Request()
	.PostAsync()

```