
The metadata header defines some basic information that JBake uses when baking the content file.

Each raw HTML or Markdown content file *must* have a metadata header in it which looks like this:

    title=Weekly Links #2
    date=2013-02-01
    type=post
    tags=weekly links, java
    status=published
    ~~~~~~
----

In the header you *must* have at least the **status** & **type** fields, the rest are optional. The only exception to this rule is if
you define a default status in your link:#configuration[configuration] file.

For an AsciiDoc formatted content file the metadata header section is optional, the JBake metadata can be defined in the AsciiDoc document header itself like so:

    = Project Structure
    Jonathan Bullock
    2013-10-17
    :jbake-type: page
    :jbake-tags: documentation, manual
    :jbake-status: published
    ----

NOTE: JBake related attributes included in the AsciiDoc header require the `jbake-` prefix to avoid any collisions.

==== Status

You have 3 options for the status field:

* `draft` - drafts are rendered the same as published content however they are given a "-draft" suffix, for example `first-post-draft.html`, but not included in any published collections
* `published`  - published content is rendered and included in the published collections
* `published-date` - providing content date is equal to or past current date content will be considered published and included in the published collections

==== Type

You can choose what template file your content file will be mixed with by changing the value of the `type` field. By default there are 2 standard types:

* `type=post` will mean the content file will be mixed with the template: post.ftl
* `type=page` will mean the content file will be mixed with the template: page.ftl

You can also define more types in your project configuration to give you more flexibility in your project, for details of this please see `<<custom_templates>>`
