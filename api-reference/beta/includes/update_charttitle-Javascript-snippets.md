
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const title = {
  overlay: true,
  text: "text-value",
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts('name')/title')
	.version('beta')
	.update({workbookChartTitle : title});

```