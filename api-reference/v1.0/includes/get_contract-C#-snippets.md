
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contract = await graphClient.Contracts
	.Request()
	.GetAsync();

```