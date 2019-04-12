# EVT Viewer Session

5th April, 2019 @ NUI Galway

## Resources

**About EVT**

_A light-weight, open source tool specifically designed to create digital editions from XML-encoded texts, freeing the scholar from the burden of web programming and enabling the final user to browse, explore and study digital editions by means of a user-friendly interface._


- EVT (Edition Visualization Technology) Viewer homepage: [http://evt.labcd.unipi.it/](http://evt.labcd.unipi.it/). Contains links to V1 and V2 demos and downloads.
- EVT2 source code: [https://github.com/evt-project/evt-viewer/](https://github.com/evt-project/evt-viewer/) 
- EVT2 Configuration tool: [http://evt.labcd.unipi.it/evt2-config/](http://evt.labcd.unipi.it/evt2-config/)
- EVT2 documentation / short-guide to EVT: [https://github.com/evt-project/evt-viewer/tree/master/app](https://github.com/evt-project/evt-viewer/tree/master/app)


## Getting up and running

1. Install Node.js and NPM. Both are contained in the installer, which you can download from [https://nodejs.org/en/](https://nodejs.org/en/) - choose the version labelled as "Recommended for Most Users". (Windows users can find some additional instructions at: [https://treehouse.github.io/installation-guides/windows/node-windows.html](https://treehouse.github.io/installation-guides/windows/node-windows.html))
2. Install `http-server` by following the [instructions to install it globally](https://github.com/indexzero/http-server#installing-globally) - type `npm install http-server -g`
3. Download a copy of the EVT 2 software from [http://evt.labcd.unipi.it](http://evt.labcd.unipi.it)
4. Unzip the folder to your desktop (or another location, if you prefer)
5. Using the command line (Terminal in Macs), change directory (use the `cd` command) to the folder containing the EVT software. If you need some help changing directories with the Command Line, there is an [interactive tutorial available on CodeAcademy](https://www.codecademy.com/learn/learn-the-command-line/modules/learn-the-command-line-navigation-u)
6. Once in the directory with the EVT files, type `http-server -c-1` - this will start your webserver and should show you an address similar to `http://127.0.0.1:8080`. You should leave this terminal window open.
7. Copy this address into your browser's address bar, and press enter 
8. Congratulations! You are now viewing a website running on your computer.

## Stopping the web server

- When you're finished working with the EVT viewer, if go back to the command line and press `ctrl` and `c`, you will stop the webserver

## Viewing your own files in EVT

1. Copy your TEI XML file into the `data` directory of EVT viewer 
2. Visit the [EVT 2 Configuration Generator](http://evt.labcd.unipi.it/evt2-config/). This is a tool used to create a file which contains the various settings the viewer needs to display your file.
3. Complete the fields appropriate to your file, and delete any unnecessary entries (such as the "Source Texts Base URL/folder" entry)
4. Once finished, in the top right of the screen, click on the "Save" button. This should prompt you to save a file named `config.json`. This file should be saved into the `config` folder of the EVT viewer.

Once you have completed these steps, return to your web-browser and refresh the page. Hopefully you are seeing your own content displayed in the viewer window.

We found during testing that experimenting with different _Edition Types_ was sometimes necessary to have the text display.