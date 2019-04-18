
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = True;

await graphClient.DirectoryObjects["{object-id}"]
	.GetMemberObjects(securityEnabledOnly)
	.Request()
	.PostAsync()

```