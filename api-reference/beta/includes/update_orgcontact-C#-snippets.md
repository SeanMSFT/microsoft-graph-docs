
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var businessPhonesList = new List<String>();
businessPhonesList.Add( "businessPhones-value" );

var contacts = new OrgContact
{
	BusinessPhones = businessPhonesList,
	City = "city-value",
	CompanyName = "companyName-value",
	Country = "country-value",
	Department = "department-value",
	DisplayName = "displayName-value",
};

await graphClient.Contacts["{id}"]
	.Request()
	.UpdateAsync(contacts);

```