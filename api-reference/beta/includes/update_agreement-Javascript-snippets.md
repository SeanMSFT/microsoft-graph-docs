
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const agreements = {
  displayName: "displayName-value",
  isViewingBeforeAcceptanceRequired: true
};

let res = await client.api('/agreements/'id'')
	.version('beta')
	.update({agreement : agreements});

```