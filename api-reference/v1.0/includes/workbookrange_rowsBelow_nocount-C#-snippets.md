
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rowsBelow = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].Range().RowsBelow()
	.Request()
	.GetAsync();

```