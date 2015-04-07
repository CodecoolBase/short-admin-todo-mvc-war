# TODO MVC

A simple TODO list application demonstrating how to build applications
using the [MVC 1.0](https://jcp.org/en/jsr/detail?id=371) specification.

## Introduction

MVC 1.0 is still at a very early stage. The final release is scheduled for Q3 2016 and will be part
of Java EE 8.

To be able to use the latest versions of all technologies which are required for MVC (like
JAX-RS, CDI and Bean Validation), this application has been created to be deployed to a 
Servlet container like [Apache Tomcat](http://tomcat.apache.org/). This allows to include
all the requirements in the WAR instead of having to rely on the container to provide these.

## Getting started

The application is pretty minimal at the moment. I'll try to add comments to the relevant
sections of the code so you don't have to read the specification for getting started. ;)

You can either deploy the WAR yourself or use the Jetty Maven plugin. In both cases
the application will be available under this URL:

    http://localhost:8080/todo-mvc/

### Build and deploy the WAR

Clone this Git repository and build the WAR using Maven:

    $ mvn clean package

The resulting WAR is named `target/todo-mvc.war`. You can now deploy this WAR file to 
[Apache Tomcat](http://tomcat.apache.org/). It is recommended to use the latest release
of the 8.0.x product line.

### Jetty Maven Plugin

Instead of deploying the WAR file yourself, you can also use the Jetty Maven plugin.
To build the project and start the embedded Jetty container, type this:

    $ mvn jetty:run-forked

## Feedback welcome

The MVC expert group is looking for feedback. Any feedback is valuable and welcome.
So if there is anything that you would like us to know, get in touch with us.

  * Post on the public [user mailing list](https://java.net/projects/mvc-spec/lists), or
  * Create an [issue](https://java.net/jira/browse/MVC_SPEC) in the issue tracker.

And remember: Now is the time to give feedback. If you don't, you cannot complain about 
it later. ;)


