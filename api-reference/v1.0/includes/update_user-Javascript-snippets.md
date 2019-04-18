
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const me = {
  accountEnabled: true,
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value"
};

let res = await client.api('/me')
	.update({user : me});

```