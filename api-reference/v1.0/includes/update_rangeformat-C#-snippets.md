
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var format = new WorkbookRangeFormat
{
	ColumnWidth = 135,
	VerticalAlignment = "Top",
	RowHeight = 49,
	WrapText = false,
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"].Range('$A$1').Format
	.Request()
	.UpdateAsync(format);

```