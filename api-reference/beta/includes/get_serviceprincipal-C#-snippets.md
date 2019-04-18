
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals["{id}"]
	.Request()
	.GetAsync();

```