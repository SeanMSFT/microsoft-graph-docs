
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroups = new CalendarGroup
{
	Name = "name-value",
};

await graphClient.Me.CalendarGroups["{id}"]
	.Request()
	.UpdateAsync(calendarGroups);

```