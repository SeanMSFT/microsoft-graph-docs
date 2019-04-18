
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var font = new WorkbookRangeFont
{
	Bold = true,
	Color = "color-value",
	Italic = true,
	Name = "name-value",
	Size = 99,
	Underline = "underline-value",
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Font
	.Request()
	.UpdateAsync(font);

```