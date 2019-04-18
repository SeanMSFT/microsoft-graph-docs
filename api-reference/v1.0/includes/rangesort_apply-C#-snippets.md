
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var icon = new WorkbookIcon
{
	Set = "set-value",
	Index = 99,
};

var fields = new WorkbookSortField
{
	Key = 99,
	SortOn = "sortOn-value",
	Ascending = true,
	Color = "color-value",
	DataOption = "dataOption-value",
	Icon = icon,
};

var fieldsList = new List<WorkbookSortField>();
fieldsList.Add( fields );

var matchCase = True;

var hasHeaders = True;

var orientation = "orientation-value";

var method = "method-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
	.Range().Sort
	.Apply(fieldsList,matchCase,hasHeaders,orientation,method)
	.Request()
	.PostAsync()

```