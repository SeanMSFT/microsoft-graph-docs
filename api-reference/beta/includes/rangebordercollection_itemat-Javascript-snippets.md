
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const borders = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/names('name')/range/format/borders/ItemAt')
	.version('beta')
	.post({workbookRangeBorder : borders});

```