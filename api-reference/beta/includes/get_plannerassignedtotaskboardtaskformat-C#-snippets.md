
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignedToTaskBoardFormat = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"].AssignedToTaskBoardFormat
	.Request()
	.GetAsync();

```