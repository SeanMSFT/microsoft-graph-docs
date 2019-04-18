
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const progressTaskBoardFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/'id'/progressTaskBoardFormat')
	.version('beta')
	.update({plannerProgressTaskBoardTaskFormat : progressTaskBoardFormat});

```