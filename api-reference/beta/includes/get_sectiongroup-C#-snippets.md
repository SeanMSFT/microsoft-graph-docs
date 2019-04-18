
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.SectionGroups["{id}"]
	.Request()
	.GetAsync();

```