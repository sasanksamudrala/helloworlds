# Introduction
HelloWorlds is an web application.

# Building the project
Building the project is as simple as:

    mvn clean install eclipse:clean eclipse:eclipse

# Running the module in local tomcat deployment.
To run in local tomcat deployment, add a tomcat server and config/dev in server classpath.
Add tomcat user role mapping to server tomcat-user.xml.

# Running the module in Tomcat
To easily run the module in Tomcat locally you can use the [tomcat7-maven-plugin](http://tomcat.apache.org/maven-plugin-2.2/tomcat7-maven-plugin/index.html) which is already configured in the **pom.xml** files, run:
    
	mvn tomcat7:run

To debug the module with the [tomcat7-maven-plugin](http://tomcat.apache.org/maven-plugin-2.2/tomcat7-maven-plugin/index.html), run:

    mvnDebug tomcat7:run

Maven will automatically wait for a debug listener on port 8000.

Then configure a remote java application and debug.
