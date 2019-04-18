
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
	.Request()
	.GetAsync();

```