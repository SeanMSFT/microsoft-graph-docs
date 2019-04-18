
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const messages = {
  isRead: "true",
};

let res = await client.api('/me/messages/{id}')
	.update({message : messages});

```