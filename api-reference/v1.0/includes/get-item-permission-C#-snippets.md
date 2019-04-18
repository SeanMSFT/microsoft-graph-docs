
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
	.Request()
	.GetAsync();

```