
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usedRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().UsedRange()
	.Request()
	.GetAsync();

```