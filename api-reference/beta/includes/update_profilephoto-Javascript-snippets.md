
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const $value = Binary data for the image;

let res = await client.api('/me/photo/$value')
	.version('beta')
	.put({Stream : $value});

```