
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

var value = new Alert
{
	AssignedTo = "String",
	ClosedDateTime = "String (timestamp)",
	Comments = commentsList,
	Feedback = AlertFeedback.Unknown,
	Id = "String (identifier)",
	Status = AlertStatus.Unknown,
	Tags = tagsList,
	VendorInformation = vendorInformation,
};

var valueList = new List<Alert>();
valueList.Add( value );

await graphClient.Security.Alerts
	.UpdateAlerts(valueList)
	.Request()
	.PostAsync()

```