
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var manager = new DirectoryObject
{
};

await graphClient.Users["{id}"].Manager
	.Request()
	.PutAsync(manager);

```