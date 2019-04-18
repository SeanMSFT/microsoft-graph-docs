
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnits = new AdministrativeUnit
{
	DisplayName = "displayName-value",
	Description = "description-value",
	Visibility = "visibility-value",
};

await graphClient.AdministrativeUnits["{id}"]
	.Request()
	.UpdateAsync(administrativeUnits);

```