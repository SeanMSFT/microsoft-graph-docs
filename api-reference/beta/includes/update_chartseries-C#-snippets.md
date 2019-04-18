
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var series = new WorkbookChartSeries
{
	Name = "name-value",
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["name"].Series["undefined"]
	.Request()
	.UpdateAsync(series);

```