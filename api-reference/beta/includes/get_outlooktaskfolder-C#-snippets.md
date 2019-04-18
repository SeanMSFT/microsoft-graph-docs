
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAAABrJAAA="]
	.Request()
	.GetAsync();

```