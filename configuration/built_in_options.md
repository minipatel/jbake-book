# Built in options

## Default assets directory

This option defines the name of the directory that holds the assets for your project.

    # folder that contains all asset files
    asset.folder=assets

## Default content directory

This option defines the name of the directory that holds the content files for your project.

    # folder that contains all content files
    content.folder=content

## Default output/destination directory

This option defines the name of the directory that will be used for the baked output to be placed in.

    # path to destination folder by default
    destination.folder=output

## Default template directory

This option defines the name of the directory that holds the template files for your project.

    # folder that contains all template files
    template.folder=templates

## Default index template file

This option defines the default template file that will be used to render the index file

    filename of masterindex template file
    template.masterindex.file=index.ftl

**WARNING:** In past releases this option was known as: `template.index.file`

==== Default archive template file

This option defines the default template file that will be used to render an archive file

    # filename of archive template file
    template.archive.file=archive.ftl

## Default feed template file

This option defines the default template file that will be used to render a feed file

    # filename of feed template file
    template.feed.file=feed.ftl

## Default sitemap template file

This option defines the default template file that will be used to render a sitemap file

    # filename of sitemap template file
    template.sitemap.file=sitemap.ftl

## Default tags template file

This option defines the default template file that will be used when rendering a file for each tag

    # filename of tag template file
    template.tag.file=tags.ftl

## Default page template file

This option defines the default template file that will be used when rendering a file of type=page

    # filename of page template file
    template.page.file=page.ftl

## Default post template file

This option defines the default template file that will be used when rendering a file of type=post

    # filename of post template file
    template.post.file=post.ftl

## Default encoding for templates

This option defines the character encoding that should be used when reading in the template files

    # character encoding MIME name used in templates.
    # use one of http://www.iana.org/assignments/character-sets/character-sets.xhtml
    template.encoding=UTF-8

## Render index file

This option defines whether an index file should be rendered or not

    # render index file?
    render.index=true

**TIP:** This option is useful when you want to use a content file as your index file allowing you to define specific content for the page instead of just using
the template.

## Render archive file

This option defines whether an archive file should be rendered or not

    # render archive file?
    render.archive=true

## Render feed file

This option defines whether a feed file should be rendered or not

    # render feed file?
    render.feed=true

## Render sitemap file

This option defines whether a sitemap file should be rendered or not

    # render sitemap.xml file?
    render.sitemap=false

## Render tag files

This option defines whether tag files are rendered or not

    # render tag files?
    render.tags=true

## Default index output filename

This option defines the output filename to be used when rendering the index file

    # filename to use for index file
    index.file=index.html

## Default archive output filename

This option defines the output filename to be used when rendering the archive file

    # filename to use for archive file
    archive.file=archive.html

## Default feed output filename

This option defines the output filename to be used when rendering the feed file

    # filename to use for feed
    feed.file=feed.xml

## Default sitemap output filename

This option defines the output filename to be used when rendering the sitemap file

    # filename to use for sitemap file
    sitemap.file=sitemap.xml

## Default tag output directory

This option defines the output directory to be used when rendering the tag files

    # folder name to use for tag files
    tag.path=tags

## Sanitize tag value

This option defines whether the tag value should be santized before being used as a filename (i.e. replace spaces with hypens)

    # sanitize tag value before it is used as filename (i.e. replace spaces with hyphens)
    tag.sanitize=false

When this option is set to true it will mean a tag value of `west wing` will be changed to `west-wing`, the tag file generated will be `west-wing.html`.

## Default encoding when rendering

This option defines the character encoding that should be used when rendering files

    # character encoding MIME name used for rendering.
    # use one of http://www.iana.org/assignments/character-sets/character-sets.xhtml
    render.encoding=UTF-8

## Default output file extension

This option defines the default file extension that should be used when rendering content files

    # file extension for output content files
    output.extension=.html

## Default suffix for draft content

This option defines the default suffix to be used when rendering draft content files

    # draft content suffix
    draft.suffix=-draft

## Default port for server mode

This option defines the default port the server will listen on

    # default server port
    server.port=8820

## Default Freemarker project file

This option defines the filename of the ZIP containing the example project that uses Freemarker templates

    # zip file containing example project structure using freemarker templates
    example.project.freemarker=example_project_freemarker.zip

## Default Groovy project file

This option defines the filename of the ZIP containing the example project that uses Groovy templates

    # zip file containing example project structure using groovy templates
    example.project.groovy=example_project_groovy.zip

## Default Thymeleaf project file

This option defines the filename of the ZIP containing the example project that uses Thymeleaf templates

    # zip file containing example project structure using thymeleaf templates
    example.project.thymeleaf=example_project_thymeleaf.zip

## Default Asciidoctor attributes

This option defines a set of default Asciidoctor attributes that are used whenever AsciiDoc formatted content is rendered

    # default asciidoctor options
    asciidoctor.attributes=source-highlighter=prettify

The value for this configuration option is a key-value pair separated by spaces, the default value defines the source highlighter that will be
used is Prettify.

## Export JBake configuration to Asciidoctor content

This option defines if the JBake configuration options should be exported to Asciidoctor as attributes so they are accessible from within AsciiDoc formatted content.

    # should JBake config options be exported to Asciidoctor engine?
    asciidoctor.attributes.export=false

**NOTE:** By default this option is disabled in default.properties

You can also define an additional prefix for the JBake configuration options, this is useful to avoid any collisions with existing AsciiDoc attributes

    # prefix that should be used when JBake config options are exported
    asciidoctor.attributes.export.prefix=

**NOTE:** By default this option is disabled in default.properties

==== Default Content Status

This option defines a default status for content files, allowing you to avoid having to define the status value in each of your content files. This value is ONLY
used if a status value hasn't been defined in the metadata header though.

    # default status
    #default.status=published

**NOTE:** By default this option is disabled in default.properties

## Default date format for content files

This option defines the default date format that is used when JBake tries to parse the date defined in the metadata header of content files.

The format is specified using pattern letters, details of what is available can be found in the
[Java API docs](https://docs.oracle.com/javase/6/docs/api/java/text/SimpleDateFormat.html).

    # default date format used in content files
    date.format=yyyy-MM-dd

## Markdown extensions

This option defines what Markdown extensions are enabled when content created in the Markdown format is rendered. Each extension required should be separated by a comma.
For details on what extensions are available please see the http://www.decodified.com/pegdown/api/org/pegdown/Extensions.html[Pegdown API docs].

    # comma delimited default markdown extensions
    markdown.extensions=HARDWRAPS,AUTOLINKS,FENCED_CODE_BLOCKS,DEFINITIONS

You can use the alias `ALL` to enable all available extensions. You can also disable specific extensions by prefixing the extension name with a hyphen:

    # comma delimited default markdown extensions
    markdown.extensions=ALL,-HARDWRAPS

## Markdown parsing timeout

This option defines the parsing timeout value in milliseconds for the Pegdown parser that is used for Markdown format support. This value limits the time spent
parsing each piece of Markdown content.

    # millis to parse single markdown page. See PegDown Parse configuration for details
    markdown.maxParsingTimeInMillis=2000

## Persistent content store

This option defines whether the content store built while parsing your content files is persisted to disk or not. When it is persisted to disk the next time you
perform a bake only those content files that have changed will be rendered speeding up the process. When it is not persisted to disk, i.e. kept in memory, a full bake
of all content is performed every time.

    # database store (local, memory)
    db.store=memory


* local = content store is persisted to disk
* memory = content store is held only in memory during bake

## Persistent content store path

This option defines the directory that is used to persist the content store to disk. It is only relevant when the content store is persisted to disk.

    # database path
    db.path=cache

## Ignore hidden asset files

This option defines whether hidden asset files should be ignored or not as part of the baking process. When set to `true` it means files such as `.DS_Store` or
`desktop.ini` won't be included in your baked output.

    asset.ignore=false
