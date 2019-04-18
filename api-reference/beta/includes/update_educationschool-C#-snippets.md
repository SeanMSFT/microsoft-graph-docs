
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = new EducationSchool
{
	DisplayName = "Fabrikam Arts High School",
	Description = "Magnate school for the arts. Los Angeles School District",
};

await graphClient.Education.Schools["10002"]
	.Request()
	.UpdateAsync(schools);

```