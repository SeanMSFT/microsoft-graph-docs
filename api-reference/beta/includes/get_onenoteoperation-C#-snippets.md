
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Me.Onenote.Operations["{id}"]
	.Request()
	.GetAsync();

```