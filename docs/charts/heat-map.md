# Heat Map

<iframe width="100%" height="550" frameborder="0" src="https://embed.plnkr.co/iyvvzBrEIayRWG5BcQ7e?show=preview">
</iframe>

# Inputs

| Property            | Type               | Default Value | Description                                                                                                     |
|---------------------|--------------------|---------------|-----------------------------------------------------------------------------------------------------------------|
| view                | number[]           |               | the dimensions of the chart [width, height]. If left undefined, the chart will fit to the parent container size |
| results             | object[]           |               | the chart data                                                                                                  |
| scheme              | object             |               | the color scheme of the chart                                                                                   |
| animations          | boolean            | true          | enable animations                                                                                               |
| legend              | boolean            | false         | show or hide the legend                                                                                         |
| legendTitle         | string             | 'Legend'      | the legend title                                                                                                |
| xAxis               | boolean            | false         | show or hide the x axis                                                                                         |
| yAxis               | boolean            | false         | show or hide the y axis                                                                                         |
| showXAxisLabel      | boolean            | false         | show or hide the x axis label                                                                                   |
| showYAxisLabel      | boolean            | false         | show or hide the y axis label                                                                                   |
| xAxisLabel          | string             |               | the x axis label text                                                                                           |
| yAxisLabel          | string             |               | the y axis label text                                                                                           |
| xAxisTickFormatting | function           |               | the x axis tick formatting                                                                                      |
| yAxisTickFormatting | function           |               | the y axis tick formatting                                                                                      |
| xAxisTicks          | any[]              |               | predefined list of x axis tick values                                                                           |
| yAxisTicks          | any[]              |               | predefined list of y axis tick values                                                                           |
| gradient            | boolean            | false         | fill elements with a gradient instead of a solid color                                                          |
| innerPadding        | number or number[] | 8             | the inner padding in px                                                                                         |
| tooltipDisabled     | boolean            | false         | show or hide the tooltip                                                                                        |
| tooltipText         | function           | (see source)  | the HTML text to display in the tooltip                                                                         |
| tooltipTemplate     | TemplateRef        |               | a custom ng-template to be displayed inside the tooltip                                                         |
| xAxisLabelSortOrder | string             | "desc"        | the x axis labels sort order.can be "","asc" or "desc"                                                          |
| yAxisLabelSortOrder | string             | "asc"         | the axis labels sort order.can be "","asc" or "desc"                                                            |
| showValueLabel      | boolean            | false         | show value labels in cell elements                                                                              |
| valueFormatting     | function           |               | the value formatting                                                                                            |

# Outputs

| Property | Description |
|----------|-------------|
| select   | click event |

# Data Format

The data format is multi series:

```
[
  {
    "name": "Germany",
    "series": [
      {
        "name": "2010",
        "value": 7300000
      },
      {
        "name": "2011",
        "value": 8940000
      }
    ]
  },

  {
    "name": "USA",
    "series": [
      {
        "name": "2010",
        "value": 7870000
      },
      {
        "name": "2011",
        "value": 8270000
      }
    ]
  }
]
```
