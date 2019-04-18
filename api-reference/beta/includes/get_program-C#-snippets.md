
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var program = await graphClient.Programs
	.Request()
	.GetAsync();

```