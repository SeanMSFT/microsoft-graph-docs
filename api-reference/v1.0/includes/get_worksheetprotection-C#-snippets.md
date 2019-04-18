
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var protection = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
	.Request()
	.GetAsync();

```