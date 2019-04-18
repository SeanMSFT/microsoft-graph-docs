
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = await graphClient.Organization
	.Request()
	.GetAsync();

```