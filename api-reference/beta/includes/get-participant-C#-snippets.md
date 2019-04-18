
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = await graphClient.App.Calls["{id}"].Participants["{id}"]
	.Request()
	.GetAsync();

```