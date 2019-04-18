
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var LastRow = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().LastRow()
	.Request()
	.GetAsync();

```