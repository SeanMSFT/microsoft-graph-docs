
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var title = new WorkbookChartAxisTitle
{
	Text = "text-value",
	Visible = true,
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["name"].Axes.ValueAxis.Title
	.Request()
	.UpdateAsync(title);

```