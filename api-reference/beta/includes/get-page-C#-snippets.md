
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pages = await graphClient.Sites["{site-id}"].Pages["{page-id}"]
	.Request()
	.GetAsync();

```