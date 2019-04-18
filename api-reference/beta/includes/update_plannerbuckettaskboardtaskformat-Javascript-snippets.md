
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const bucketTaskBoardFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat')
	.version('beta')
	.update({plannerBucketTaskBoardTaskFormat : bucketTaskBoardFormat});

```