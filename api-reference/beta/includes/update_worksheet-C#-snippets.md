
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var worksheets = new WorkbookWorksheet
{
	Position = 99,
	Name = "name-value",
	Visibility = "visibility-value",
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
	.Request()
	.UpdateAsync(worksheets);

```