
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var range = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["{index}"].Range()
	.Request()
	.GetAsync();

```