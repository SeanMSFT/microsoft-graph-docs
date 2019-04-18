
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sort = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Sort
	.Request()
	.GetAsync();

```