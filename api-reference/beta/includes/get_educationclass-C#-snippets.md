
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Classes["11023"]
	.Request()
	.GetAsync();

```