
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = new Message
{
	IsRead = "true",
};

await graphClient.Me.Messages["{id}"]
	.Request()
	.UpdateAsync(messages);

```