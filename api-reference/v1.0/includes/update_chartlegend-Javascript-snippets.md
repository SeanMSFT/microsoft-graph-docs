
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const legend = {
  visible: true,
  position: "position-value",
  overlay: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
	.update({workbookChartLegend : legend});

```