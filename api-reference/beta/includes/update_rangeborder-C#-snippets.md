
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var borders = new WorkbookRangeBorder
{
	Color = "color-value",
	Style = "style-value",
	SideIndex = "sideIndex-value",
	Weight = "weight-value",
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().Format.Borders["sideIndex"]
	.Request()
	.UpdateAsync(borders);

```