# Maven coordinates
The main JBake artifact is available from the Maven Central repository, these are the coordinates:

    <dependency>
    	<groupId>org.jbake</groupId>
    	<artifactId>jbake-core</artifactId>
    	<version>2.4.0</version>
    </dependency>

The 3rd party libraries that provide support for Markdown content or the Freemarker template engine etc. are defined as optional dependencies in `jbake-core` so if
you plan on using them you will have to include them as a dependency in your project as well.

For Markdown content support add the following dependency:


    <dependency>
    	<groupId>org.pegdown</groupId>
    	<artifactId>pegdown</artifactId>
    	<version>1.4.2</version>
    </dependency>


For AsciiDoc content support add the following dependency:


    <dependency>
    	<groupId>org.asciidoctor</groupId>
    	<artifactId>asciidoctorj</artifactId>
    	<version>1.5.2</version>
    </dependency>


For Freemarker template support add the following dependency:


    <dependency>
    	<groupId>org.freemarker</groupId>
    	<artifactId>freemarker</artifactId>
    	<version>2.3.20</version>
    </dependency>

For Groovy template support add the following dependencies:

    <dependency>
        <groupId>org.codehaus.groovy</groupId>
        <artifactId>groovy</artifactId>
        <version>2.3.6</version>
    </dependency>
    <dependency>
        <groupId>org.codehaus.groovy</groupId>
        <artifactId>groovy-templates</artifactId>
        <version>2.3.6</version>
    </dependency>

For Thymeleaf template support add the following dependencies:

    <dependency>
    	<groupId>org.thymeleaf</groupId>
    	<artifactId>thymeleaf</artifactId>
    	<version>2.1.3.RELEASE</version>
    </dependency>
    <dependency>
    	<groupId>org.thymeleaf.extras</groupId>
    	<artifactId>thymeleaf-extras-conditionalcomments</artifactId>
    	<version>2.1.1.RELEASE</version>
    </dependency>

