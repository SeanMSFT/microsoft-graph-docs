
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const points = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts('name')/series('undefined')/points/ItemAt')
	.version('beta')
	.post({workbookChartPoint : points});

```