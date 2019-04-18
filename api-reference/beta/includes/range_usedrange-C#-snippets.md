
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var UsedRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["name"].Range().UsedRange()
	.Request()
	.GetAsync();

```