
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var font = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().Format.Font
	.Request()
	.GetAsync();

```