
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Schools["10001"]
	.Request()
	.GetAsync();

```