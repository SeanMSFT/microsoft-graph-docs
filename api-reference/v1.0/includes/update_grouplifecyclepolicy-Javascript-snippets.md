
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicies = {
  groupLifetimeInDays: 180,
  managedGroupTypes: "Selected",
  alternateNotificationEmails: "admin@contoso.com"
};

let res = await client.api('/groupLifecyclePolicies/{id}')
	.update({groupLifecyclePolicy : groupLifecyclePolicies});

```