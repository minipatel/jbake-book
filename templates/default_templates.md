# Default Templates
There are default template files defined in JBake that are used to render a number of special pages that require no content files to be present, these are:

* `index` - used to render an index.html file
* `archive` - used to render an archive.html file
* `feed` - used to render a feed.xml file
* `tag` - used to render a HTML file for each tag used
* `sitemap` - used to render a sitemap.xml file

If you don't require any of these special pages to be rendered then you can turn off the rendering of them by adding the following lines to your
`jbake.properties` file:


    render.index=false
    render.archive=false
    render.feed=false
    render.tags=false
    render.sitemap=false


There are also two default templates files defined in JBake that are used to render content files, these are:

* `page` - used to render any content file marked with a type of 'page'
* `post` - used to render any content file marked with a type of 'post'
