
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const photo = {
  height: 99,
  width: 99,
  id: "id-value"
};

let res = await client.api('/users/{id|userPrincipalName}/photo')
	.version('beta')
	.update({profilePhoto : photo});

```