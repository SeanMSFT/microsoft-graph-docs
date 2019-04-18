
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usedRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].UsedRange(true)
	.Request()
	.GetAsync();

```