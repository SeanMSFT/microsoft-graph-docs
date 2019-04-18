
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.CalendarGroups["{id}"]
	.Request()
	.DeleteAsync();

```