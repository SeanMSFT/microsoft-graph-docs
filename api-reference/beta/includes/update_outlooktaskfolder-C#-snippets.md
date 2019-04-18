
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = new OutlookTaskFolder
{
	Name = "Charity work",
};

await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAhrbPWAAA="]
	.Request()
	.UpdateAsync(taskFolders);

```