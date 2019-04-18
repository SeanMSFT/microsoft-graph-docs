
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Classes["{class-id}"]
	.Request()
	.GetAsync();

```