
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const plans = {
  title: "title-value"
};

let res = await client.api('/planner/plans/'id'')
	.version('beta')
	.update({plannerPlan : plans});

```