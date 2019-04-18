
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var progressTaskBoardFormat = await graphClient.Planner.Tasks["{task-id}"].ProgressTaskBoardFormat
	.Request()
	.GetAsync();

```