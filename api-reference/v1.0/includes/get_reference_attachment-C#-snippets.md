
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Events["{id}"].Attachments["{id}"]
	.Request()
	.GetAsync();

```