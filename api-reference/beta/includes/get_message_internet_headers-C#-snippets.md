
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages["AAMkAGVmMDEz"]
	.Request()
	.Select( e => new {
			 e.InternetMessageHeaders 
			 })
	.GetAsync();

```