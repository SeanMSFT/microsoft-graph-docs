
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityActions = await graphClient.Security.SecurityActions["{id}"]
	.Request()
	.GetAsync();

```