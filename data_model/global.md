# Global

These data variables are available to all templates regardless.

- `version` = version of JBake being used
- `published_date` = date baking took place
- `[type]s` = collection of all content of [type] (e.g. posts = all content of type=post or snippets = all content of type=snippet)
- `published_content` = collection of all published content (regardless of the type)
- `published_posts` = collection of just published posts in date descending order
- `published_pages` = collection of just published pages in date descending order
- `all_content` = collection of all content (regardless of type)
- `alltags` = collection of all tags used across all content
- `content.rootpath` = path to root of project (to be used for relative path to assets)
- `config.[option]` = map of configuration data

All the configuration options are available with any `.` in the property being replaced with `_`.
For example `template.index.file=index.ftl` is available via `config.template_index_file`.

In your templates you can loop through any of the collections above in the templates, and access a map of values for each element like so: `content.[value]`
all of the metadata header fields are available such as `content.title` along with the body of the content file `content.body`.

////
Include example on how to loop in Freemarker
////
