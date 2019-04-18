
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const manager = {
  @odata.id: "https://graph.microsoft.com/v1.0/users/{id}"
};

let res = await client.api('/users/{id}/manager/$ref')
	.put({directoryObject : manager});

```