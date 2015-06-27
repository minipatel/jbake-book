# Page / Post / Custom
These predefined templates as well as any custom templates you create yourself have the following data available to them:

- `content.[value]` = map of file contents

All of the metadata header fields are available such as `content.title` and the body of the file is available via `content.body`.

In the map you also have access to:

- `content.file` = the full path to the source file
- `content.uri` = the URI for the baked file
