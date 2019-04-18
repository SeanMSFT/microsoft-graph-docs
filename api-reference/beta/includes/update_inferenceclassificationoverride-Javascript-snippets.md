
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const overrides = {
  classifyAs: "focused"
};

let res = await client.api('/me/inferenceClassification/overrides/{id}')
	.version('beta')
	.update({inferenceClassificationOverride : overrides});

```