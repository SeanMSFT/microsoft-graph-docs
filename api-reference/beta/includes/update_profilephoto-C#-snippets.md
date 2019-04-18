
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var $value = "Binary data for the image"

await graphClient.Me.Photo.Content
	.Request()
	.PutAsync($value);

```