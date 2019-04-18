
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fill = new WorkbookRangeFill
{
	Color = "#0000FF",
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$C$1').Format.Fill
	.Request()
	.UpdateAsync(fill);

```