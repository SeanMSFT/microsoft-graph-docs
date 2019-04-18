
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const content = The contents of the file goes here.;

let res = await client.api('/me/drive/items/{item-id}/content')
	.put({Stream : content});

```