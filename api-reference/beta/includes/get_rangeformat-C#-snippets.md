
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var format = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().Format
	.Request()
	.GetAsync();

```