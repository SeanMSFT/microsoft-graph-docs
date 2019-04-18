
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domains = await graphClient.Domains["contoso.com"]
	.Request()
	.GetAsync();

```