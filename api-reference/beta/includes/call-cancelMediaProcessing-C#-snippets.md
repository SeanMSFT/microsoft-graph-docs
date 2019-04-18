
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var all = True;

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
	.CancelMediaProcessing(all,clientContext)
	.Request()
	.PostAsync()

```