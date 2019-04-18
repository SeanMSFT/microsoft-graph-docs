
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrencies = await graphClient.BookingCurrencies["USD"]
	.Request()
	.GetAsync();

```