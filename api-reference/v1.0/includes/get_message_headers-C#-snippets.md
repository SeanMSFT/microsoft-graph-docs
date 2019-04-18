
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages["AAMkADhAAAW-VPeAAA="]
	.Request()
	.Select( e => new {
			 e.InternetMessageHeaders 
			 })
	.GetAsync();

```