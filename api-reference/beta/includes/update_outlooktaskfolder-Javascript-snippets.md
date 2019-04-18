
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const taskFolders = {
  name: "Charity work"
};

let res = await client.api('/me/outlook/taskFolders('AAMkADIyAAAhrbPWAAA=')')
	.version('beta')
	.update({outlookTaskFolder : taskFolders});

```