
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var vendorInformation = new SecurityVendorInformation
{
	Provider = "String",
	Vendor = "String",
};

var tagsList = new List<String>();
tagsList.Add( "String" );

var commentsList = new List<String>();
commentsList.Add( "String" );

var alerts = new Alert
{
	AssignedTo = "String",
	ClosedDateTime = "String (timestamp)",
	Comments = commentsList,
	Feedback = AlertFeedback.Unknown,
	Status = AlertStatus.Unknown,
	Tags = tagsList,
	VendorInformation = vendorInformation,
};

await graphClient.Security.Alerts["{alert_id}"]
	.Request()
	.UpdateAsync(alerts);

```