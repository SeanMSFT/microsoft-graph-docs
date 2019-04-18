
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupTypesList = new List<String>();
groupTypesList.Add( "groupTypes-value" );

var groups = new Group
{
	Description = "description-value",
	DisplayName = "displayName-value",
	GroupTypes = groupTypesList,
	Mail = "mail-value",
	MailEnabled = true,
	MailNickname = "mailNickname-value",
};

await graphClient.Groups["{id}"]
	.Request()
	.UpdateAsync(groups);

```