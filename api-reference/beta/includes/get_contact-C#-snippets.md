
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts["AAMkAGI2THk0AAA="]
	.Request()
	.GetAsync();

```