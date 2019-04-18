
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Buckets["{bucket-id}"]
	.Request()
	.GetAsync();

```