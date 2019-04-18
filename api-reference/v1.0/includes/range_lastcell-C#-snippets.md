
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lastCell = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().LastCell()
	.Request()
	.GetAsync();

```