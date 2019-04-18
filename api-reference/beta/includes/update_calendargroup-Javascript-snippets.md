
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const calendarGroups = {
  name: "name-value"
};

let res = await client.api('/me/calendarGroups/{id}')
	.version('beta')
	.update({calendarGroup : calendarGroups});

```