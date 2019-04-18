
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = new IdentityProvider
{
	ClientSecret = "1111111111111",
};

await graphClient.IdentityProviders["Amazon-OAuth"]
	.Request()
	.UpdateAsync(identityProviders);

```