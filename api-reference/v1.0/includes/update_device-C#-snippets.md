
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = new Device
{
	AccountEnabled = false,
};

await graphClient.Devices["{id}"]
	.Request()
	.UpdateAsync(devices);

```