
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alternativeSecurityIds = new AlternativeSecurityId
{
	Type = 99,
	IdentityProvider = "identityProvider-value",
	Key = "key-value",
};

var alternativeSecurityIdsList = new List<AlternativeSecurityId>();
alternativeSecurityIdsList.Add( alternativeSecurityIds );

var device = new Device
{
	AccountEnabled = true,
	AlternativeSecurityIds = alternativeSecurityIdsList,
	ApproximateLastSignInDateTime = "2016-10-19T10:37:00Z",
	DeviceId = "deviceId-value",
	DeviceMetadata = "deviceMetadata-value",
	DeviceVersion = 99,
};

await graphClient.Devices
	.Request()
	.AddAsync(device);

```