
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var minorGridlines = new WorkbookChartGridlines
{
	Visible = true,
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["name"].Axes.ValueAxis.MinorGridlines
	.Request()
	.UpdateAsync(minorGridlines);

```