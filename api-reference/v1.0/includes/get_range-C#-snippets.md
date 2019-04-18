
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var range = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range()
	.Request()
	.GetAsync();

```