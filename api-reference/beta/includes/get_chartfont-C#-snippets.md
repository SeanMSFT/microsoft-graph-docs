
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var font = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["name"].Axes.ValueAxis.Format.Font
	.Request()
	.GetAsync();

```