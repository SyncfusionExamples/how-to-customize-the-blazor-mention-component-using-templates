# How to customize the Blazor Mention Component using templates

A quick start Blazor project that shows how to customize the Blazor Mention component using templates. This project also includes a code snippet to bind a remote data source to the Blazor Mention component.

Refer to the following documentation to learn about the Blazor Mention component:
https://blazor.syncfusion.com/documentation/mention/templates

Check out this online example of the Blazor Mention component:
https://blazor.syncfusion.com/demos/mention/template?theme=fluent

Watch the following video to get started with a Blazor Web Assembly app and add Syncfusion Blazor components to it:
https://www.youtube.com/watch?v=zKU580cOqjg

## Project prerequisites
Make sure that you have the compatible versions of [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) (17.14 or later) and the [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) installed before starting to work on this project.

## How to run this application
Clone this repository and open it in Visual Studio 2022. Build and run the project to view the output.

From the command line:

```
dotnet run
```

## Database dependency
This sample does not use LocalDB, SQL Server, Entity Framework, or any other database. Weather data on the Fetch data page is read from the static file `wwwroot/sample-data/weather.json`. The Mention sample binds templates and a commented remote `SfDataManager` URL; no external service is required to load the page.
