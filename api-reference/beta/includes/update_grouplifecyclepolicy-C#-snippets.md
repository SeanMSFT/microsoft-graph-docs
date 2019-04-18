
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicies = new GroupLifecyclePolicy
{
	GroupLifetimeInDays = 180,
	ManagedGroupTypes = "Selected",
	AlternateNotificationEmails = "admin@contoso.com",
};

await graphClient.GroupLifecyclePolicies["{id}"]
	.Request()
	.UpdateAsync(groupLifecyclePolicies);

```