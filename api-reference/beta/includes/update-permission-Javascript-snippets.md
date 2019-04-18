
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const permissions = {
  roles: [ "read" ]
};

let res = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
	.version('beta')
	.update({permission : permissions});

```