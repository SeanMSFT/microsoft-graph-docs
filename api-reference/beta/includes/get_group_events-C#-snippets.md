
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var event = await graphClient.Groups["{id}"].Events
	.Request()
	.GetAsync();

```