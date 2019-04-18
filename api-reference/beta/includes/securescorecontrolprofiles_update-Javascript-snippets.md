
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const secureScoreControlProfiles = {
  assignedTo: "assignedTo-value",
  controlStateUpdates: "controlStateUpdates-value",
  tenantNote: "tenantNote-value"
};

let res = await client.api('/security/secureScoreControlProfiles/AdminMFA')
	.version('beta')
	.update({secureScoreControlProfile : secureScoreControlProfiles});

```