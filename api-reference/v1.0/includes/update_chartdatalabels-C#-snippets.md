
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataLabels = new WorkbookChartDataLabels
{
	Position = "position-value",
	ShowValue = true,
	ShowSeriesName = true,
	ShowCategoryName = true,
	ShowLegendKey = true,
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].DataLabels
	.Request()
	.UpdateAsync(dataLabels);

```