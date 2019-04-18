
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const items = {
  name: "new-file-name.docx"
};

let res = await client.api('/me/drive/items/{item-id}')
	.version('beta')
	.update({driveItem : items});

```