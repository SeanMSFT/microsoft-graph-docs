
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataPolicyOperations = await graphClient.DataPolicyOperations["{id}"]
	.Request()
	.GetAsync();

```