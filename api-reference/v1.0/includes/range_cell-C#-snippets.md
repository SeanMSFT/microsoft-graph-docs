
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cell = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Cell(5,6)
	.Request()
	.GetAsync();

```