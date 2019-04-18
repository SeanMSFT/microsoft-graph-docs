
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = new EducationClass
{
	Description = "History - World History 1",
	DisplayName = "World History Level 1",
};

await graphClient.Education.Classes["11014"]
	.Request()
	.UpdateAsync(classes);

```