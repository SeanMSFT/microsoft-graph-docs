
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const settings = {
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/settings/{id}')
	.version('beta')
	.update({directorySetting : settings});

```