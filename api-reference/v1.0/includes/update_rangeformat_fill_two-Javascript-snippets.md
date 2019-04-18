
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const fill = {
  color: "#00FF00"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill')
	.update({workbookRangeFill : fill});

```