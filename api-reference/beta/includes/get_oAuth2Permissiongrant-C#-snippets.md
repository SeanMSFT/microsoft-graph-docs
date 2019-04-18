
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2Permissiongrants = await graphClient.OAuth2Permissiongrants["{id}"]
	.Request()
	.GetAsync();

```