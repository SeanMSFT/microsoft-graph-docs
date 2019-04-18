
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const series = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts('name')/series/ItemAt')
	.version('beta')
	.post({workbookChartSeries : series});

```