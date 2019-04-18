
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = new ConversationThread
{
	IsLocked = true,
};

await graphClient.Groups["{id}"].Threads["{id}"]
	.Request()
	.UpdateAsync(threads);

```