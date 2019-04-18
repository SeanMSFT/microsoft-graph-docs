
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusinesses = await graphClient.BookingBusinesses["Fabrikam@M365B489948.onmicrosoft.com"]
	.Request()
	.GetAsync();

```