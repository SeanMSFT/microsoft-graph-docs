
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = True;

await graphClient.DirectoryObjects["{object-id}"]
	.GetMemberGroups(securityEnabledOnly)
	.Request()
	.PostAsync()

```