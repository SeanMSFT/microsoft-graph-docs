
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const messageRules = Content-type: application/json

{
    displayName: "Important from partner",
    actions: {
        markImportance: "high"
     }
};

let res = await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')')
	.version('beta')
	.update({messageRule : messageRules});

```