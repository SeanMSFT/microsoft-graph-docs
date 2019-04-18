
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const oAuth2Permissiongrants = {
  scope: "scope-value"
};

let res = await client.api('/oAuth2Permissiongrants/{id}')
	.version('beta')
	.update({oAuth2PermissionGrant : oAuth2Permissiongrants});

```