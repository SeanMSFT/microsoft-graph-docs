
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Schools["{school-id}"]
	.Request()
	.GetAsync();

```