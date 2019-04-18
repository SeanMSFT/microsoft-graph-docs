
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = new Application
{
	AllowPublicClient = false,
	DisplayName = "New display name",
};

await graphClient.Applications["{id}"]
	.Request()
	.UpdateAsync(applications);

```