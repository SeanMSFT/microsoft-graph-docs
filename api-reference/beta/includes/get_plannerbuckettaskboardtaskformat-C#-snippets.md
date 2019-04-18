
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bucketTaskBoardFormat = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"].BucketTaskBoardFormat
	.Request()
	.GetAsync();

```