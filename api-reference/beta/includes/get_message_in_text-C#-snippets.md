
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages["AAMkAGI1AAAoZCfHAAA="]
	.Request()
	.Header("Prefer","outlook.body-content-type="text"")
	.Select( e => new {
			 e.Subject,
			 e.Body,
			 e.BodyPreview,
			 e.UniqueBody 
			 })
	.GetAsync();

```