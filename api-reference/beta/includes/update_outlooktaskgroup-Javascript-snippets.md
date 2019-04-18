
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const taskGroups = Content-type: application/json
Content-length: 28

{
  name: "Personal Tasks",
};

let res = await client.api('/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')')
	.version('beta')
	.update({outlookTaskGroup : taskGroups});

```