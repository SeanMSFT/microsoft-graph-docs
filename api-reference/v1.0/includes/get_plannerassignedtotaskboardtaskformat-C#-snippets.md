
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignedToTaskBoardFormat = await graphClient.Planner.Tasks["{task-id}"].AssignedToTaskBoardFormat
	.Request()
	.GetAsync();

```