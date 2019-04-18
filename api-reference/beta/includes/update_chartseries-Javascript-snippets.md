
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const series = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts('name')/series('undefined')')
	.version('beta')
	.update({workbookChartSeries : series});

```