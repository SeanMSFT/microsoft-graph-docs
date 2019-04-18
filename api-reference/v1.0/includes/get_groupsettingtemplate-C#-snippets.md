
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplates = await graphClient.GroupSettingTemplates["{id}"]
	.Request()
	.GetAsync();

```