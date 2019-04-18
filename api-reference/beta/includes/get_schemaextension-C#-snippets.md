
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtensions = await graphClient.SchemaExtensions["graphlearn_test"]
	.Request()
	.GetAsync();

```