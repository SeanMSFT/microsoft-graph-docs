
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var progressTaskBoardFormat = await graphClient.Planner.Tasks["'id'"].ProgressTaskBoardFormat
	.Request()
	.GetAsync();

```