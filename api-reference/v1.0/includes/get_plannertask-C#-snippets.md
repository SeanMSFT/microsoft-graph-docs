
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Tasks["{task-id}"]
	.Request()
	.GetAsync();

```