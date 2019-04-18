
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "Sheet1!A1:D5";

var hasHeaders = True;

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
	.Add(address,hasHeaders)
	.Request()
	.PostAsync()

```