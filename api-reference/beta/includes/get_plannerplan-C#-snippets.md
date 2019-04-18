
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Planner.Plans["'id'"]
	.Request()
	.GetAsync();

```