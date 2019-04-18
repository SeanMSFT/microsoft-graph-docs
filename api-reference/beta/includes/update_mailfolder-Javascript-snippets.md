
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const mailFolders = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
	.version('beta')
	.update({mailFolder : mailFolders});

```