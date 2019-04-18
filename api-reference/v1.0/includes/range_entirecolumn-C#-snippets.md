
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entireColumn = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().EntireColumn()
	.Request()
	.GetAsync();

```