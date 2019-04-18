
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var range = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Range('A1:B2')
	.Request()
	.GetAsync();

```