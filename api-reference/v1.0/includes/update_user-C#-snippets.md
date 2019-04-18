
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var businessPhonesList = new List<String>();
businessPhonesList.Add( "businessPhones-value" );

var me = new User
{
	AccountEnabled = true,
	BusinessPhones = businessPhonesList,
	City = "city-value",
};

await graphClient.Me
	.Request()
	.UpdateAsync(me);

```