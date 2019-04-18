
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const fields = {
    Color: "Fuchsia",
    Quantity: 934
};

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/fields')
	.update({fieldValueSet : fields});

```