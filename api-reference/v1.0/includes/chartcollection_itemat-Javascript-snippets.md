
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const charts = {
  index: 8
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt')
	.post({workbookChart : charts});

```