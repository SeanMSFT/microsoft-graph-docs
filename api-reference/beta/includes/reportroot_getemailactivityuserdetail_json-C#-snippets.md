
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailActivityUserDetail = await graphClient.Reports.GetEmailActivityUserDetail('D7')
	.Request()
	.GetAsync();

```