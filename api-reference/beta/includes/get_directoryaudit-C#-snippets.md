
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudits = await graphClient.AuditLogs.DirectoryAudits["{id}"]
	.Request()
	.GetAsync();

```