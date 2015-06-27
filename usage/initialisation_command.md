# Initialisation command

The server command will allow you to see what your baked site looks like when served out by a HTTP web server, great for when you want to preview your site using
your local web browser.

The `-s` option will start JBake in server mode allowing you to preview your baked site at http://localhost:8820/ by default it will serve out the contents of the
`output` directory in the current working directory:


    $ jbake -s


NOTE: The local port used can be changed via the configuration file.

You can specify the directory to serve out by supplying an additional parameter:


    $ jbake -s <directory>

