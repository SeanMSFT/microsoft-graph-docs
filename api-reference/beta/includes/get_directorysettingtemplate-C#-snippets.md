
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplates = await graphClient.DirectorySettingTemplates["{id}"]
	.Request()
	.GetAsync();

```