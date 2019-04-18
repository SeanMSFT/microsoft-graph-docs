
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const fill = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
	.update({workbookRangeFill : fill});

```