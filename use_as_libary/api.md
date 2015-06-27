# API

The main class you should be focusing on using is `Oven`, this class provides the main functionality via a `.bake()` method that requires some parameters to be
passed to it. Here's an example:


    try {
    	File source = new File("/path/to/project_source"); //<1>
    	File destination = new File("/path/to/project_output"); //<2>
    	Oven oven = new Oven(source, destination, true); //<3>
    	oven.setupPaths(); //<4>
    	oven.bake(); //<5>
    } catch (JBakeException e) { //<6>
    	// do something with exception here
    }


<1> Defines the project source, this should be the root directory of the project, JBake will look in this directory for `jbake.properties`
<2> Defines where the baked output should be placed
<3> The third parameter defines if the local cache (persistent content store) should be cleared and therefore trigger a full bake
<4> This method checks the paths supplied exist and content the required elements
<5> This method performs the actual baking
<6> If any exceptions are thrown during the path checks or baking they are wrapped in a JBakeException
