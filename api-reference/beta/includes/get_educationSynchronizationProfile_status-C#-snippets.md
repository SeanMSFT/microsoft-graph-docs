
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileStatus = await graphClient.Education.SynchronizationProfiles["{id}"].ProfileStatus
	.Request()
	.GetAsync();

```