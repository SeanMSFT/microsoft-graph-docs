
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var uploadUrl = await graphClient.Education.SynchronizationProfiles["{id}"].UploadUrl()
	.Request()
	.GetAsync();

```