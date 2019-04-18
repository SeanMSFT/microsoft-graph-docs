
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var education = await graphClient.Education
	.Request()
	.GetAsync();

```