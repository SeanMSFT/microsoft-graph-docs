
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "A1:D8";

var hasHeaders = False;

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
	.Add(address,hasHeaders)
	.Request()
	.PostAsync()

```