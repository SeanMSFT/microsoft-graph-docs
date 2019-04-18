
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages["AAMkADYAAAImV_lAAA="]
	.Request()
	.GetAsync();

```