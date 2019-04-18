
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rolesList = new List<String>();
rolesList.Add( "read" );

var permissions = new Permission
{
	Roles = rolesList,
};

await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
	.Request()
	.UpdateAsync(permissions);

```