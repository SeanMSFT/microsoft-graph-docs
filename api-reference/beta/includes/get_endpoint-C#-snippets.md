
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Groups["{id}"].Endpoints["{id}"]
	.Request()
	.GetAsync();

```