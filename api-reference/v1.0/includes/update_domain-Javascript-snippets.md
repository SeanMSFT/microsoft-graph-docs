
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const domains = {
  isDefault: true,
  supportedServices: [
    "Email",
    "OfficeCommunicationsOnline"
  ]
};

let res = await client.api('/domains/contoso.com')
	.update({domain : domains});

```