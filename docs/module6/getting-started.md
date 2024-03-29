# Getting started

## Preparing the test environment

This section will cover how to test locally a Potree web page before deploying it to a server.

Due to strict security policies in browsers, it is not possible to open potree html files directly on your pc because potree needs permission to load files. You have to put all necessary source files and the pointcloud on a webserver to view the result. You can, however, install a local webserver on your pc. [XAMPP](https://www.apachefriends.org/index.html), which contains Apache Webserver as well as PHP and MySQL, is the suggested solution for testing locally potree pages.

After you’ve installed and started Apache/XAMPP, you can access files in your htdocs directory through a localhost URL. Assuming your htdocs directory is *C:xampphtdocs*, you can access it in your browser with:

` http://localhost `

## Choosing a text editor

This module is strongly focused in coding, despite if no prior knowledge of HTML, CSS and JS is needed. For this reason, a proper and efficient text editor is highly recommended. We suggest to use **[Visual Studio Code](https://github.com/microsoft/vscode)** with Prettier extension installed.
