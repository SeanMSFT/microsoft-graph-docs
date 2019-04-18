
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new Json
{
};

var names = new WorkbookNamedItem
{
	Type = "type-value",
	Scope = "scope-value",
	Comment = "comment-value",
	Value = value,
	Visible = true,
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
	.Request()
	.UpdateAsync(names);

```