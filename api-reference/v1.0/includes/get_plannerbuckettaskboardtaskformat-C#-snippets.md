
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bucketTaskBoardFormat = await graphClient.Planner.Tasks["{task-id}"].BucketTaskBoardFormat
	.Request()
	.GetAsync();

```