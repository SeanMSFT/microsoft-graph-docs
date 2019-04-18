
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var protection = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().Format.Protection
	.Request()
	.GetAsync();

```