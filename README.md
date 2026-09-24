# How to Change the Position of the Axis in Blazor Chart

## Overview

This sample demonstrates how to change the default placement of chart axes in Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts). The implementation uses the `OpposedPosition` property on both the primary X-axis and primary Y-axis to render the axes on the opposite side of the chart area.

Changing axis placement is useful when aligning chart layouts with specific reporting requirements, improving readability, or matching visualization standards used within business dashboards. The sample displays weather report data in a column chart and shows how axis positioning can be customized without changing the underlying data source.

## Key Features

- Uses the `SfChart` component to render the chart.
- Configures `ChartPrimaryXAxis` with:
  - `ValueType="Syncfusion.Blazor.Charts.ValueType.Category"`
  - `OpposedPosition="true"`
- Configures `ChartPrimaryYAxis` with:
  - `OpposedPosition="true"`
- Displays data using a `ChartSeries` configured with:
  - `DataSource="@WeatherReports"`
  - `XName="X"`
  - `YName="Y"`
  - `Type="ChartSeriesType.Column"`
- Demonstrates axis repositioning without modifying the chart data model.
- Uses a strongly typed `ChartData` class containing `X` and `Y` properties.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the `AxisPosition.csproj` project.
3. Restore NuGet packages when prompted.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory:

```bash
cd AxisPosition
```

4. Restore NuGet packages:

```bash
dotnet restore
```

5. Run the application:

```bash
dotnet run
```

6. Open the local URL displayed in the terminal after the application starts.

## Project Structure


`AxisPosition/Pages/Index.razor` — Sample page containing the `SfChart`, axis configuration, data model, and chart series implementation.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the Syncfusion Chart axis customization documentation: https://help.syncfusion.com/chart-sdk/blazor/charts/axis-customization

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.