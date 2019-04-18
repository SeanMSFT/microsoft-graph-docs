
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var overrides = new InferenceClassificationOverride
{
	ClassifyAs = InferenceClassificationType.Focused,
};

await graphClient.Me.InferenceClassification.Overrides["{id}"]
	.Request()
	.UpdateAsync(overrides);

```