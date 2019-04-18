
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const minorGridlines = {
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts('name')/axes/valueaxis/minorgridlines')
	.version('beta')
	.update({workbookChartGridlines : minorGridlines});

```