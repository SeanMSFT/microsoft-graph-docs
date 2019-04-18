
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var templates = new SynchronizationTemplate
{
	Id = "Slack",
	ApplicationId = "{id}",
	FactoryTag = "CustomSCIM",
};

await graphClient.Applications["{id}"].Synchronization.Templates["{templateId}"]
	.Request()
	.PutAsync(templates);

```