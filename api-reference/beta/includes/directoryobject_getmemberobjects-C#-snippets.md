
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = True;

await graphClient.Me
	.GetMemberObjects(securityEnabledOnly)
	.Request()
	.PostAsync()

```