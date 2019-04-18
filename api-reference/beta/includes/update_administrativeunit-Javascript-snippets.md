
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const administrativeUnits = {
  displayName: "displayName-value",
  description: "description-value",
  visibility: "visibility-value"
};

let res = await client.api('/administrativeUnits/{id}')
	.version('beta')
	.update({administrativeUnit : administrativeUnits});

```