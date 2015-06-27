# Templates Directory

The templates directory is where your templates files go, these files are "mixed" with your content files to generate the baked output. You should place your
templates into the root of this directory.

The extension of the template file determines the template engine:

* `.ftl` = [Freemarker](http://freemarker.org)
* `.gsp` = [Groovy's SimpleTemplateEngine](http://www.groovy-lang.org/)
* `.groovy` = [Groovy's SimpleTemplateEngine](http://www.groovy-lang.org/)
* `.gxml` = [Groovy's XmlTemplateEngine](http://www.groovy-lang.org/)
* `.thyme` = [Thymeleaf](http://www.thymeleaf.org/)
* `.html` = [Thymeleaf](http://www.thymeleaf.org/)

It is recommended that you don't mix different template types, try to stick to just 1 type of templates in your project.

For more information on what you can do in each template engine have a look at the example templates provided with JBake and their
respective documentation: [Freemarker](http://freemarker.org/docs/index.html), [Groovy](http://docs.groovy-lang.org/latest/html/documentation/template-engines.html) &
[Thymeleaf](http://www.thymeleaf.org/doc/html/Using-Thymeleaf.html).
