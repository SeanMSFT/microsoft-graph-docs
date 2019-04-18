
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var details = await graphClient.Planner.Tasks["{task-id}"].Details
	.Request()
	.GetAsync();

```