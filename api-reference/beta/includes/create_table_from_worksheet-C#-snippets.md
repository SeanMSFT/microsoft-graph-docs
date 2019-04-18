
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "";

var hasHeaders = False;

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Tables
	.Add(address,hasHeaders)
	.Request()
	.PostAsync()

```