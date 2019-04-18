
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages["AAMkADYAAAImV_jAAA="]
	.Request()
	.Expand("eventMessage/event")
	.GetAsync();

```