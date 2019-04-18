
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var posts = await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"]
	.Request()
	.GetAsync();

```