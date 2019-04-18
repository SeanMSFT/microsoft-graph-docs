
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var event = await graphClient.Me.CalendarView
	.Request()
	.GetAsync();

```