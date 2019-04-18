
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var items = new DriveItem
{
	Name = "new-file-name.docx",
};

await graphClient.Me.Drive.Items["{item-id}"]
	.Request()
	.UpdateAsync(items);

```