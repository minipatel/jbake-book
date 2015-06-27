# Content Body

You can also define custom metadata in the header that can be exposed to the templates, for example:

    summary=This is a summary of the larger post

And access it in the templates like so:
    <p>${content.summary}</p>

This feature is extremely useful when you want to control the rendering of extra market in the templates such as [Disqus](https://disqus.com) for comments
on certain posts/pages or to display images using some JavaScript library like [jQuery](https://jquery.com/)

==== Complex Custom Metadata

If you need to define a complex structure of metadata you can use JSON format to achieve this, here's an example:

    type=page
    og={"description": "Something"}


WARNING: The JSON content must be contained within a single line and cannot span multiple lines.

This complex data is then accessible from the templates like this:


    <#if content?? && content.og??> <1>
	    <meta property="og:description" content="${content.og.description}"/> <2>
    </#if>


<1> Checks the `content` map is not null and that the `content.og` map is not null
<2> Outputs the `description` value from the `content.og` map

=== Content Body

Everything after the metadata header is considered the content body and made available to the templates, after being converted to HTML if required in the case of
Markdown or AsciiDoc.
