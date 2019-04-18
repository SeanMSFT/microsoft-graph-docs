
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legend = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Legend
	.Request()
	.GetAsync();

```