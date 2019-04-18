
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreements = await graphClient.Agreements["'id'"]
	.Request()
	.Expand("files")
	.GetAsync();

```