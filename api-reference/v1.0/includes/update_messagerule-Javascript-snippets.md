
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const messageRules = {
    displayName: "Important from partner",
    actions: {
        markImportance: "high"
     }
};

let res = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
	.update({messageRule : messageRules});

```