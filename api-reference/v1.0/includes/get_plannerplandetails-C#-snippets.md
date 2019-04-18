
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var details = await graphClient.Planner.Plans["{plan-id}"].Details
	.Request()
	.GetAsync();

```