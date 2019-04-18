
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var LastCell = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().LastCell()
	.Request()
	.GetAsync();

```