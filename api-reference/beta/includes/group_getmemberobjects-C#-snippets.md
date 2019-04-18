
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = False;

await graphClient.Groups["{id}"]
	.GetMemberObjects(securityEnabledOnly)
	.Request()
	.PostAsync()

```