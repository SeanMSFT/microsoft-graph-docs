
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const devices = {
  accountEnabled: false
};

let res = await client.api('/devices/{id}')
	.update({device : devices});

```