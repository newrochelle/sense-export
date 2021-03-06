# sense-export
> Just a simple button to export data in your Qlik Sense application without displaying them in a table first.

![](https://raw.githubusercontent.com/stefanwalther/sense-export/master/docs/images/sense-export.png)

---
## Table of Contents
- [Purpose and Description](#purpose-and-description)
- [Screenshots](#screenshots)
- [Installation & Download](#installation--download)
- [Configuration](#configuration)
- [Compatibility](#compatibility)
- [Known Issues](#known-issues)
- [Contributing](#contributing)
- [Related Projects](#related-projects)
- [Author](#author)
- [License](#license)

_(TOC generated by [verb](https://github.com/verbose/verb) using [markdown-toc](https://github.com/jonschlinkert/markdown-toc))_

---

## Purpose and Description
***sense-export*** is a tiny and sweet visualization extension allowing you to **export data without showing the underlaying table**. 

### Why?
Every object in Qlik Sense provides the export functionality, but sometimes one just wants to provide a download of some data from your data model by putting a tiny little button onto a screen, completely without showing the data first

## Screenshots

Just a very simple button with some properties to define the layout and the behavior of the export.
See **Configuration** for mor details.

![](https://raw.githubusercontent.com/stefanwalther/sense-export/master/docs/images/all-props.png)

## Installation & Download
1. Download the [latest version](https://github.com/stefanwalther/sense-export/raw/master/build/sense-export_latest.zip) or [any other version](https://github.com/stefanwalther/sense-export/tree/master/build) you want to install.
2. Then install on either *Qlik Sense Desktop* or *Qlik Sense Server*:

* Qlik Sense Desktop
	* To install, unzip all files and copy the content to the folder folder `"C:\Users\%USERNAME%\Documents\Qlik\Sense\Extensions\sense-navigation"`
* Qlik Sense Server
	* See instructions [how to import an extension on Qlik Sense Server](http://help.qlik.com/sense/2.0/en-US/online/#../Subsystems/ManagementConsole/Content/import-extensions.htm)

## Configuration
## Dimensions & Measures

Define dimensions and measures as you would do for every other extension.
Pro Tip: Enable the debug mode if you want to see the result.

## Button label

- **Label** - Just define the label of the button, defaults to "Export".

![](https://raw.githubusercontent.com/stefanwalther/sense-export/master/docs/images/prop-label.png)

## Button layout

The possibilities to layout the button should (hopefully) be pretty self-explanatory:

- **Style** - Select on of the predefined styles.
- **Button width** - Define whether the button should take the full width of the object or not.
- **Alignment** - Define the **horizontal** alignment.
- **Icon** - Select one of the provided icons. Defaults to "download"
Pro Tip: Font Awesome icons are used here, go to https://fortawesome.github.io/Font-Awesome/icons/ to get a nice overview of all icons possible.

![](https://raw.githubusercontent.com/stefanwalther/sense-export/master/docs/images/prop-export-definition.png)

## Export definition

Define the final output of the export:

- **Format** - Select on of the following values: 1) Open XML (Excel), 2) Comma separated CSV, 3) Tab separated CSV; defaults ot "Open XML (Excel)"
- **State** - You can define whether your current selection will be considered or not. If this is the desired behavior, select "Possible values", otherwise "All values", then always all data will be exported, regardless the current selections.
- **File name** - Optionally you can define a file name.

![](https://raw.githubusercontent.com/stefanwalther/sense-export/master/docs/images/prop-export-definition.png)

## Debug
While working in edit mode it's quite helpful to test the data (which will then be exported in the defined format).
If you enable the debug mode a debug table will be shown to double-check if you you have defined the correct measures and dimensions.

Note:
- The debug table will only be shown in edit mode, even if this settings is activated
- The debug table only shows the first 500 records (for performance reasons). The export will contain all data, though.

![](https://raw.githubusercontent.com/stefanwalther/sense-export/master/docs/images/prop-debug.png)

## Compatibility
***sense-export*** is designed to work with Qlik Sense 2.1.1 or higher.
If you use the visualization extension in an older version of Qlik Sense the following message will be shown:

![](https://raw.githubusercontent.com/stefanwalther/sense-export/master/docs/images/unsupported.png)

## Known Issues
There are two known issues which will be addressed in future versions:

- Vertical alignment of the button is currently now possible.
- Improvement for the mobile view, reserve less space for the export button.

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/stefanwalther/sense-export/issues).
The process for contributing is outlined below:

1. Create a fork of the project
2. Work on whatever bug or feature you wish
3. Create a pull request (PR)

I cannot guarantee that I will merge all PRs but I will evaluate them all.

## Related Projects
Some related projects (Qlik Sense Visualization Extensions) I have recently created:

- [qliksense-extension-tutorial](https://www.npmjs.com/package/qliksense-extension-tutorial): Comprehensive tutorial to start developing Qlik Sense Extensions. | [homepage](https://github.com/stefanwalther/qliksense-extension-tutorial "Comprehensive tutorial to start developing Qlik Sense Extensions.")
- [sense-calendar-heatmap](https://www.npmjs.com/package/sense-calendar-heatmap): Qlik Sense Visualization Extension with a diverging color scale. The values are displayed as colored… [more](https://github.com/stefanwalther/qsCalendarHeatmap) | [homepage](https://github.com/stefanwalther/qsCalendarHeatmap "Qlik Sense Visualization Extension with a diverging color scale. The values are displayed as colored cells per day. Days are arranged into columns by week, then grouped by month and years.")
- [sense-extension-recipes](https://www.npmjs.com/package/sense-extension-recipes): Recipes on working with Qlik Sense Visualization Extensions. | [homepage](https://github.com/stefanwalther/sense-extension-recipes "Recipes on working with Qlik Sense Visualization Extensions.")
- [sense-funnel-chart](https://www.npmjs.com/package/sense-funnel-chart): Funnel Chart for Qlik Sense. | [homepage](https://github.com/stefanwalther/sense-funnel-chart "Funnel Chart for Qlik Sense.")
- [sense-media-box](https://www.npmjs.com/package/sense-media-box): Include web pages, videos, images and much more into your Qlik Sense app. | [homepage](https://github.com/stefanwalther/sense-media-box "Include web pages, videos, images and much more into your Qlik Sense app.")
- [sense-navigation](https://www.npmjs.com/package/sense-navigation): Sense Sheet Navigation + Actions visualization extension for Qlik Sense. | [homepage](https://github.com/stefanwalther/sense-navigation#readme "Sense Sheet Navigation + Actions visualization extension for Qlik Sense.")
- [sense-on-off-switch](https://www.npmjs.com/package/sense-on-off-switch): Set a variable in Qlik Sense to true/false using an on-off switch. | [homepage](https://github.com/stefanwalther/sense-on-off-switch "Set a variable in Qlik Sense to true/false using an on-off switch.")
- [sense-qr-code](https://www.npmjs.com/package/sense-qr-code): QR Code to be embedded into Qlik Sense. | [homepage](https://github.com/stefanwalther/qsQRCode "QR Code to be embedded into Qlik Sense.")
- [sense-range-slider](https://www.npmjs.com/package/sense-range-slider): Slider object for Qlik Sense to manipulate one or two variables. | [homepage](https://github.com/QlikDev/qsRangeSlider "Slider object for Qlik Sense to manipulate one or two variables.")
- [sense-themable-kpi-tile](https://www.npmjs.com/package/sense-themable-kpi-tile): KPI Tile for Qlik Sense with the ability to use themes or to customize background… [more](https://github.com/stefanwalther/sense-themable-kpi-tile) | [homepage](https://github.com/stefanwalther/sense-themable-kpi-tile "KPI Tile for Qlik Sense with the ability to use themes or to customize background color, comparison indicator, etc.")  

## Author
**Stefan Walther**
* [qliksite.io](http://qliksite.io)
* [twitter/waltherstefan](http://twitter.com/waltherstefan)
* [github.com/stefanwalther](http://github.com/stefanwalther)

## License
Released under the MIT license.

***

_This file was generated by [verb](https://github.com/verbose/verb), v0.9.0, on July 26, 2016._

