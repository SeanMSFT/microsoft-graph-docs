
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const buckets = {
  name: "Development"
};

let res = await client.api('/planner/buckets/{bucket-id}')
	.update({plannerBucket : buckets});

```