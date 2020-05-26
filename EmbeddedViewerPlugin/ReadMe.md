# EmbeddedViewerPlugin

A simple ICN plug-in that implements a thin wrapper around the ICN Content Viewer widget. The plug-in allows the content viewer to be loaded as a stand-alone ICN feature, suitable for presentation in a custom application. A basic JavaScript function is provided for opening one or more documents in this ContentViewer widget.

## Prerequisites

* IBM Content Navigator
* [Apache Ant](http://ant.apache.org/)

## Installation
A EmbeddedViewerPlugin JAR file is available for use in the root directory. It can also be built by following these steps:

1. Download the EmbeddedViewerPlugin from [GitHub](https://github.com/ibm-ecm/ibm-content-navigator-samples/tree/master/EmbeddedViewerPlugin).
2. Create a **lib** directory under the EmbeddedViewerPlugin.
3. Add the navigatorAPI.jar and j2ee.jar file to the **lib** directory, and update the **classpath** in the build.xml to point to the **lib** directory.
4. Build the JAR file by running Apache Ant.

    ```
    C:\> cd C:\EmbeddedViewerPlugin
    C:\EmbeddedViewerPlugin> ant
    ```

## How to use this plugin
Embedded Content Viewer Plugin is available to ICN as a feature. Example of other features are Browsing, Searching and Administration. Features are URL-addressable, hence when loading ICN, it is possible to specify the feature ID as a request parameter, to have that feature opened directly when loading ICN. To facilitate seamless integration, there is also a request parameter that allows for the window dressing of the application to be hidden.

In order to enble this fesature, go to Administrator in ICN, create a seperate desktop called "demo". After assigning the proper repository, go to layout tab and deselect all feature but "ICN Content Viewer". Save and close. This feature can then be accessed by appending desktop parameter: "&desktop=demo".

## Additional references

* [EmbeddedViewer Plugin Part I](https://www.ibm.com/support/pages/node/1280704?lang=en)
* [EmbeddedViewer Plugin Part II](https://www.ibm.com/support/pages/node/1280698?lang=en)
* [Developing applications with IBM Content Navigator](https://www.ibm.com/support/knowledgecenter/SSEUEX_3.0.7/com.ibm.developingeuc.doc/eucdi000.html)
* [dW Answers forum](https://developer.ibm.com/answers/topics/icn/)