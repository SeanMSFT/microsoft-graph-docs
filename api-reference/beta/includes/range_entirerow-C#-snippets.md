
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var EntireRow = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().EntireRow()
	.Request()
	.GetAsync();

```