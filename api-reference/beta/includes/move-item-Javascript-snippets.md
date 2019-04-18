
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const items = {
  parentReference: {
    id: "new-parent-folder-id"
  },
  name: "new-item-name.txt"
};

let res = await client.api('/me/drive/items/{item-id}')
	.version('beta')
	.update({driveItem : items});

```