
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const charts = {
  height: 99,
  left: 99
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts('name')')
	.version('beta')
	.update({workbookChart : charts});

```