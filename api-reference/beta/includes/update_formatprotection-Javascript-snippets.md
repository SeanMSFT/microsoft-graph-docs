
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const protection = {
  locked: true,
  formulaHidden: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names('name')/range/format/protection')
	.version('beta')
	.update({workbookFormatProtection : protection});

```