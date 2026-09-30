# How to Customize the Blazor Mention Component Using Templates

## Overview

This sample demonstrates how to customize the Syncfusion [Blazor Mention](https://www.syncfusion.com/blazor-components/blazor-mention) component using template-based rendering. The application displays mention suggestions with additional user information such as profile images, names, and email addresses, enabling a more informative and visually rich user experience than a standard text-only suggestion list.

The sample uses custom item and display templates to personalize how mention data is presented within the suggestion popup. It also includes a remote data binding example, showing how Mention suggestions can be populated from external data sources. This approach is useful for collaboration, social, messaging, CRM, helpdesk, and productivity applications that require user tagging and identification features.

## Key Features

- Integrates the Syncfusion Blazor Mention component (`SfMention<TItem>`) with the Syncfusion Rich Text Editor (`SfRichTextEditor`) for user mention functionality.
- Uses the `Target` property to connect the Mention component to the Rich Text Editor content area.
- Configures the Mention suggestion popup using:
  - `PopupHeight="200px"`
  - `PopupWidth="350px"`
- Maps mention display values through `MentionFieldSettings` using the `FirstName` field of the `EmployeeData` model.
- Demonstrates custom loading content through the `SpinnerTemplate`.
- Displays custom empty-state content using the `NoRecordsTemplate`.
- Includes custom CSS styling and animated loading indicator using CSS keyframes.
- Contains a sample Weather Forecast page that demonstrates:
  - Dependency injection with `HttpClient`.
  - Loading JSON data from `wwwroot/sample-data/weather.json`.
  - Asynchronous data retrieval using `GetFromJsonAsync<T>()`.
  - Rendering fetched data in a tabular UI.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the project file:

   `BlazorApp__Mention.csproj`

3. Restore NuGet packages.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open an integrated terminal and navigate to the project directory.
3. Restore NuGet packages:

```bash
dotnet restore
```

4. Run the application:

```bash
dotnet run
```

5. Open the local URL displayed in the terminal after the application starts.

## Project Structure

- `Pages/Index.razor` - Primary sample showcasing Syncfusion Mention integration with the Rich Text Editor, custom templates, popup configuration, and mention field mapping.
- `Pages/FetchData.razor` - Demonstrates loading weather forecast data from a local JSON file using `HttpClient` and rendering the results in a table.
- `Shared/SurveyPrompt.razor` - Reusable component demonstrating parameterized content using the `[Parameter]` attribute.
- `wwwroot/sample-data/weather.json` - Local JSON data source consumed by `Pages/FetchData.razor`.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Official documentation: https://blazor.syncfusion.com/documentation/mention/templates

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.