Version Exporter for Photoshop
==============================

![Main Window](https://raw.github.com/thommeo/Version-Exporter/master/docs/Documentation/Images/Main%20Window.png)

Version Exporter is a script for Adobe Photoshop to help you export LayerComps or LayerSets (Folders or Groups) as separate files and wrap them with Safari, Firefox or generic flat browser window.

## Download

Download Version Exporter from Adobe Creative Cloud:
https://creative.adobe.com/addons/products/8042

## Description

Supported formats for exported files: JPG, PSD, PNG, TIFF.

Supported browser window wraps: Safari, Firefox, Generic Flat.

Add your own window title and URL for the Browser Wrap.

If you want transparent background behind the browser window, leave the Background color field empty and set the file type to PNG, PSD or TIFF.

Macros for the filename template:
* Use {document} for the current document name
* Use {name} for the current Version name (LayerComp or LayerSet name)
* Use {####} for the number of the Version being exported. Number of "#" determine number of digits including leading zeros.
* Use strftime formatting for current date and time. E.g. "%Y-%m-%d" will give you current date in format YYYY-MM-DD

Short tutorial:
* Open "company_homepage.psd" file with your design
* Create there 2 LayerComps called "Default" and "Navigation Open"
* Launch Version Exporter script from File -> Scripts -> Version Exporter
* Put the following in the filename template field "{document}_%Y-%m-%d_{##}_{name}"
* Select "Use Comps as versions" in the "Operation Mode" dropdown
* Hit "Run" button
This will result in 2 JPG files:
* company_homepage_2015-02-23_01_Default.jpg
* company_homepage_2015-02-23_02_Navigation Open.jpg

Automate your exports with flexible configuration:
https://github.com/thommeo/Version-Exporter/blob/master/docs/Documentation/Manual.md#project-configuration

Read more about the functionality:
https://github.com/thommeo/Version-Exporter/blob/master/docs/Documentation/Manual.md

## Change Log

1.2.3

* Updated README and documentation

1.2.2

* Fixed bug with Safari Wrap
* Firefox Wrap and Flat wrap now leave the source contents editable in a SmartObject as well

1.2.1

* Safari Wrap now leaves the actual content in the SmartObjects instead of merging the document.

## License

https://github.com/thommeo/Version-Exporter/blob/master/docs/EULA.txt

