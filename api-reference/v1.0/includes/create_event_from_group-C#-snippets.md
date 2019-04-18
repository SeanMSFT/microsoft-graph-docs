
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var responseStatus = new ResponseStatus
{
	Response = ResponseType.None,
	Time = "datetime-value",
};

var event = new Event
{
	OriginalStartTimeZone = "originalStartTimeZone-value",
	OriginalEndTimeZone = "originalEndTimeZone-value",
	ResponseStatus = responseStatus,
	ICalUId = "iCalUId-value",
	ReminderMinutesBeforeStart = 99,
	IsReminderOn = true,
};

await graphClient.Groups["{id}"].Events
	.Request()
	.AddAsync(event);

```