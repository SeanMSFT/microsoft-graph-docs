
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = await graphClient.Me.Drive.Items["{id}"].Workbook.Application
	.Request()
	.GetAsync();

```