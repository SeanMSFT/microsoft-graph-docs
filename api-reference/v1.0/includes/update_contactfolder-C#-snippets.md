
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolders = new ContactFolder
{
	ParentFolderId = "parentFolderId-value",
	DisplayName = "displayName-value",
};

await graphClient.Me.ContactFolders["{id}"]
	.Request()
	.UpdateAsync(contactFolders);

```