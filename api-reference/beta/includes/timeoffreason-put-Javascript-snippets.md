
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const timeOffReasons = {
  displayName: "Vacation",
  iconType: "plane",
  isActive: true
};

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
	.version('beta')
	.put({timeOffReason : timeOffReasons});

```