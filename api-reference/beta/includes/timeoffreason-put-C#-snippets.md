
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReasons = new TimeOffReason
{
	DisplayName = "Vacation",
	IconType = TimeOffReasonIconType.Plane,
	IsActive = true,
};

await graphClient.Teams["{teamId}"].Schedule.TimeOffReasons["{timeOffReasonId}"]
	.Request()
	.PutAsync(timeOffReasons);

```