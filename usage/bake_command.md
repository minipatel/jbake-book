# Bake command

The bake command mixes your source content with your templates and cooks it all into a fully baked web site. You have a number of different ways to execute the bake
command to suite your requirements.

The `-b` option without any parameters will assume your source content is in the current working directory and will place the baked output into a directory named `output`
in the current directory:


    $ jbake -b


**NOTE:** JBake will create this `output` directory if it does not already exist.

If you specify only the source directory as a parameter then the output directory will automatically be generated inside the source directory:


    $ jbake -b <source>


You can also specify your source directory and output directory to enable you to have full control over the baking process:


    $ jbake -b <source> <output>


You can even omit the `-b` option as bake is the default command for the command line interface of JBake:


    $ jbake <source> <output>


You can even go as far to omit all options and parameters to execute the bake command:


    $ jbake


**NOTE:** Again JBake will assume your source content is in the current working directory will place the baked output into `output`.
