
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shifts = await graphClient.Teams["{teamId}"].Schedule.Shifts["{shiftId}"]
	.Request()
	.GetAsync();

```