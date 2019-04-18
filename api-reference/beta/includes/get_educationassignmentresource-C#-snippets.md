
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.Education.Classes["11021"].Assignments["19002"].Resources["22002"]
	.Request()
	.GetAsync();

```