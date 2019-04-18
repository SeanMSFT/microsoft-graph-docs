
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var details = await graphClient.Planner.Plans["xqQg5FS2LkCp935s-FIFm2QAFkHM"].Details
	.Request()
	.GetAsync();

```