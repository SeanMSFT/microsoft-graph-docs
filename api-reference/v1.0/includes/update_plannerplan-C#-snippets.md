
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = new PlannerPlan
{
	Title = "title-value",
};

await graphClient.Planner.Plans["{plan-id}"]
	.Request()
	.UpdateAsync(plans);

```