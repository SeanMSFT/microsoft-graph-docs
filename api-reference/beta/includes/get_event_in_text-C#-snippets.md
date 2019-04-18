
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Events["AAMkAGI1AAAoZDOFAAA="]
	.Request()
	.Header("Prefer","outlook.body-content-type="text"")
	.Select( e => new {
			 e.Subject,
			 e.Body,
			 e.BodyPreview 
			 })
	.GetAsync();

```