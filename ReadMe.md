# Sample RestDSL Project using Camel-Boot and Docker

This example demonstrates a RestDSL frontend to a couple of simple routes.  It runs in a Java standalone container, using Spring with Apache Camel.

This example is implemented using solely a Spring XML file (there is no custom Java code).

### Building

The example can be built with

    mvn clean install


### Running the example locally

The example can be run locally using the following Maven goal:

    mvn exec:java


### Running the example in Docker

It is assumed that Docker is already running on your local build machine. 

The example can be built and deployed using a single goal:

    mvn -Pf8-deploy

To run the example using docker, use the following command:

    docker run -it --rm -p 8080:8080 fabric8/sample-spring:0.0.1-SNAPSHOT

### More details

You can find more details about running this [quickstart](http://fabric8.io/guide/quickstarts/running.html) on the website. This also includes instructions how to change the Docker image user and registry.

