
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites["{site-id}"]
	.Request()
	.GetAsync();

```