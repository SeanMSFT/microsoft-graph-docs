
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var details = await graphClient.Planner.Tasks["gcrYAaAkgU2EQUvpkNNXLGQAGTtu"].Details
	.Request()
	.GetAsync();

```