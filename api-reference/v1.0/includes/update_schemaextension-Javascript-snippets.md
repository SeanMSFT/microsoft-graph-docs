
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const schemaExtensions = {
  properties: [
    {
      name:"new-name-value",
      type:"new-type-value"
    },
    {
      name:"additional-name-value",
      type:"additional-type-value"
    }
  ],
};

let res = await client.api('/schemaExtensions/{id}')
	.update({schemaExtension : schemaExtensions});

```