
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var LastColumn = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().LastColumn()
	.Request()
	.GetAsync();

```