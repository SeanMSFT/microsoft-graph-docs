
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.IdentityProviders["Amazon-OAuth"]
	.Request()
	.GetAsync();

```