
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = await graphClient.ServicePrincipals["{servicePrincipalId}"].Synchronization.Jobs["{jobId}"].Schema
	.Request()
	.Header("Authorization","Bearer {Token}")
	.GetAsync();

```