
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const line = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line')
	.update({workbookChartLineFormat : line});

```