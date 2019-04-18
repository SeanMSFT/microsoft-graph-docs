
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = True;

await graphClient.Me.Drive.Items["{id}"].Workbook
	.CreateSession(this,persistChanges)
	.Request()
	.PostAsync()

```