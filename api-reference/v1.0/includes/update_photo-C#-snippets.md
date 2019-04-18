
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var photo = new ProfilePhoto
{
	Height = 99,
	Width = 99,
	Id = "id-value",
};

await graphClient.Users["{id|userPrincipalName}"].Photo
	.Request()
	.UpdateAsync(photo);

```