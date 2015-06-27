# Content Directory
The content directory is where your content files should be placed, these files will be "mixed" with the templates to generate the baked output. Again
you can create any directory structure you like for your content, this structure will be maintained when the baked output is created.

The extension of the content file determines what type of content it contains:

* `.html` = raw HTML content
* `.md` = [Markdown](http://daringfireball.net/projects/markdown/syntax) formatted content
* `.ad` = [AsciiDoc](http://www.methods.co.nz/asciidoc/) formatted content
* `.adoc` = [AsciiDoc](http://www.methods.co.nz/asciidoc/) formatted content
* `.asciidoc` = [AsciiDoc](http://www.methods.co.nz/asciidoc/) formatted content

**NOTE:** JBake uses [Pegdown](http://pegdown.org) to support Markdown format and [Asciidoctor](http://asciidoctor.org/) to support AsciiDoc format.
