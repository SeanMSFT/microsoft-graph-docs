
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskGroups = await graphClient.Me.Outlook.TaskGroups["AAMkADIyAAAhrbe-AAA="]
	.Request()
	.GetAsync();

```