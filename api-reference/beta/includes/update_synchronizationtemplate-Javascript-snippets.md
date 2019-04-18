
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const templates = {
    id: "Slack",
    applicationId: "{id}",
    factoryTag: "CustomSCIM"
};

let res = await client.api('/applications/{id}/synchronization/templates/{templateId}')
	.version('beta')
	.put({synchronizationTemplate : templates});

```