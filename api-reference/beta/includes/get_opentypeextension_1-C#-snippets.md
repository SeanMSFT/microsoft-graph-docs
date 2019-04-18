
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extensions = await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions["Com.Contoso.Referral"]
	.Request()
	.GetAsync();

```