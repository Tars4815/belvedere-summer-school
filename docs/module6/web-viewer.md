# 3D Viewer implementation

In order to start designing the web page that is going to host the Potree-based viewer, start creating a new folder within *C:\xampp\htdocs*. Name it according to the name you want to associate to the url. For example, if you'll name it *belvedere-example*, when you'll access the test web page you will have to search for *localhost/belvedere-example* on the browser.

The folder you have just created will contain all the files and assets needed to enable the Potree viewer. In particular:

* **index.html**: this file with HTML extension will be the homepage of the 3D web viewer, containing the basic settings for the GUI and including the paths to additional external files for style (css) and/or functionalities (js).

* **libs** folder: it contains many subfolders for all libraries' dependencies for making functionable the viewer.

* **licenses** folder: it includes license specifications for the libraries used in the development.

* **css** folder: it contains file(s) that define the style and appearance of the web page.

* **js** folder: this includes all the scripting JavaScript files that enable native and/or custom functionalities and actions on the web page.

* **pointclouds** folder: inside this space converted pointclouds are saved with their ancillary files.

* **img_selected** folder: it containes oriented images that the viewer developer is willing to integrate on the platform. Together with the picture files, camera certificates and images orientation parameters are saved in this folder.

## Defining *index.html*

The index.html file includes the main settings for the web page that contains the custom Potree viewer. At the top of the file, the doctype declaration for HTML file is included as follows:

```
 <!DOCTYPE html>
```

Hence, the root of the page is initialised with the `html` tag, that includes the other main tag of an html page - `head` and `body` - as well as the indication to the browser on how to interprete the language of the text in the page.

```
<html lang="en">
<head>
    ...
</head>
<body>
    ...
</body>
</html>  
```

The head tag houses the metadata of your website. For example, information contained in this part defines the title that will appear on the browser window when the page is loaded as well as other important metadata regarding the content and/or the author(s) of the page. Connection to stylesheets (.css files) are also inserted here. Most of the information inserted will remain invisible to normal visitors of the page but represent relevant information for browsers and search engines.

These settings need to be defined in the first lines in the head element as follows:

```
<head>
    <!-- Specifying the character encoding for the document -->
	<meta charset="utf-8">
    <!-- Providing a shrt description for the page content -->
	<meta name="description" content="Simple Potree viewer">
    <!-- Specifying the author of the document -->
	<meta name="author" content="Your name here">
    <!-- Declaring needed information for website responsivity -->
	<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <!-- Setting the title of the page -->
	<title>Belvedere glacier</title>
    <!--Linking the needed stylesheet of the libraries adopted in the rest of the code-->
	<link rel="stylesheet" type="text/css" href="./libs/potree/potree.css">
	<link rel="stylesheet" type="text/css" href="./libs/jquery-ui/jquery-ui.min.css">
	<link rel="stylesheet" type="text/css" href="./libs/openlayers3/ol.css">
	<link rel="stylesheet" type="text/css" href="./libs/spectrum/spectrum.css">
	<link rel="stylesheet" type="text/css" href="./libs/jstree/themes/mixed/style.css">
</head>
```

**[..UNDER CONSTRUCTION..]**