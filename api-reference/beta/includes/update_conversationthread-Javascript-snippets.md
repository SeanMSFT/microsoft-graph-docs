
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const threads = {
  @odata.type:"#Microsoft.OutlookServices.ConversationThread",
  isLocked: true
};

let res = await client.api('/groups/{id}/threads/{id}')
	.version('beta')
	.update({conversationThread : threads});

```