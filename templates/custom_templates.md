# Custom Templates
You also have the ability to define new custom templates that can be used when rendering different types of content files.

First add the following line to your `jbake.properties` file:


    template.<customtype>.file=templateXYZ.ftl


Then create your template file and place it into the 'templates' folder inside your project, after that you can create your content files making sure
that the metadata header has the following entry:

    type=<customtype>


If you'd like the content files to be rendered with your custom template file using a different extension then add the following to your `jbake.properties` file:


    template.<customtype>.extension=.xml

