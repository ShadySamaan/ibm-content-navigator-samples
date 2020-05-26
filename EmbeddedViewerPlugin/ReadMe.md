# EmbeddedViewerPlugin

The EmbeddedViewer Plugin also known as Content Viewer widget which is available in IBM Content Navigator, presents a tabbed viewing user interface, where multiple documents can be opened. In this widget, each document is opened within a new tab. However, options are available for splitting/opening a second copy of the tabs either vertically or horizontally. This makes it possible to open two different documents side-by-side.

The EmbeddedViewer Plugin widget also provides access to view the document properties, or to add comments to a document – where supported. The widget has the capability to recognize when a document requested to be viewed is already opened in a tab. Instead of opening a new tab, the widget brings the correct tab to the foreground. For more information, follow the link in the [additional references](#additional-references) section.

## Prerequisites

* IBM Content Navigator
* J2EE library
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

* [EmbeddedViewer Plugin](https://www.ibm.com/support/pages/node/1280704?lang=en)
* [Developing applications with IBM Content Navigator](https://www.ibm.com/support/knowledgecenter/SSEUEX_3.0.7/com.ibm.developingeuc.doc/eucdi000.html)
* [dW Answers forum](https://developer.ibm.com/answers/topics/icn/)