
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const valueAxis = {
  majorUnit: {
  },
  maximum: {
  },
  minimum: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis')
	.update({workbookChartAxis : valueAxis});

```