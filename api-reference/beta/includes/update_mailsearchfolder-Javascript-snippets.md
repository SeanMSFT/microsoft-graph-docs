
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const mailFolders = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  filterQuery: "contains(subject, 'Analytics')))"
};

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
	.version('beta')
	.update({mailFolder : mailFolders});

```