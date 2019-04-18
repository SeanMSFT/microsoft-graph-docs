
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
	.Request()
	.GetAsync();

```