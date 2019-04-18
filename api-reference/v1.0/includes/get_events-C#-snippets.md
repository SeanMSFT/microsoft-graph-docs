
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var event = await graphClient.Me.Events
	.Request()
	.Header("Prefer","outlook.timezone="Pacific Standard Time"")
	.Select( e => new {
			 e.Subject,
			 e.Body,
			 e.BodyPreview,
			 e.Organizer,
			 e.Attendees,
			 e.Start,
			 e.End,
			 e.Location 
			 })
	.GetAsync();

```