
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var minimum = new Json
{
};

var maximum = new Json
{
};

var majorUnit = new Json
{
};

var valueAxis = new WorkbookChartAxis
{
	MajorUnit = majorUnit,
	Maximum = maximum,
	Minimum = minimum,
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis
	.Request()
	.UpdateAsync(valueAxis);

```