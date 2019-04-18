
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = new PlannerBucket
{
	Name = "Development",
};

await graphClient.Planner.Buckets["{bucket-id}"]
	.Request()
	.UpdateAsync(buckets);

```