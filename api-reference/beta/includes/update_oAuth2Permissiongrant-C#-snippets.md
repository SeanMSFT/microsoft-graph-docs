
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2Permissiongrants = new OAuth2PermissionGrant
{
	Scope = "scope-value",
};

await graphClient.OAuth2Permissiongrants["{id}"]
	.Request()
	.UpdateAsync(oAuth2Permissiongrants);

```