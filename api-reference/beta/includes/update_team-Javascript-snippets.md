
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const teams = {
  memberSettings: {
    allowCreateUpdateChannels: true
  },
  messagingSettings: {
    allowUserEditMessages: true,
    allowUserDeleteMessages: true
  },
  funSettings: {
    allowGiphy: true,
    giphyContentRating: "strict"
  }
};

let res = await client.api('/teams/{id}')
	.version('beta')
	.update({team : teams});

```