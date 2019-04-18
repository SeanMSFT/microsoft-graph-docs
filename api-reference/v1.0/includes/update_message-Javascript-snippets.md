
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const messages = {
  subject: "subject-value",
  body: {
    contentType: "",
    content: "content-value"
  },
  inferenceClassification: "other"
};

let res = await client.api('/me/messages/{id}')
	.update({message : messages});

```