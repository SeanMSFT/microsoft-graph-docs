
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shares = await graphClient.Shares["{shareIdOrEncodedSharingUrl}"]
	.Request()
	.GetAsync();

```