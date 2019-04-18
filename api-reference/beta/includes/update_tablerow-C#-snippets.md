
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = new WorkbookTableRow
{
	Index = 99,
	Values = "values-value",
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["index"]
	.Request()
	.UpdateAsync(rows);

```