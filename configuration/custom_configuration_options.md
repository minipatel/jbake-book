# Custom configuration options
You can also define additional options in your `jbake.properties` file for use in your project, especially in your template files. A great example is provided in the
sample projects that have an option called `site.host` which defines the host URL for the site:

    site.host=http://jbake.org

This custom option is then used from within the feed template like so:

    ...
    <title><#escape x as x?xml>${post.title}</#escape></title>
    <link>${config.site_host}/${post.uri}</link>
    <pubDate>${post.date?string("EEE, d MMM yyyy HH:mm:ss Z")}</pubDate>
    ...


To provide an absolute URI for use in a link.
