
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroups = await graphClient.Me.CalendarGroups["{id}"]
	.Request()
	.GetAsync();

```