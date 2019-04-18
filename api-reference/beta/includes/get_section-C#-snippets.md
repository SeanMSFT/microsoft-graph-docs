
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Sections["{id}"]
	.Request()
	.GetAsync();

```