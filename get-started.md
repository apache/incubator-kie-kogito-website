---
layout: get-started
title: Get Started
permalink: /get-started/
---

# Run the examples

<div class="blue uppercase">This guide covers, Downloading the Kogito examples, Building and running one of the Kogito examples, and Testing the running example with some REST requests.</div>

## Download Kogito examples

To download a released version of the Kogito examples, visit [this page](https://github.com/kiegroup/kogito-examples/releases) and select the latest version of the kogito-examples. Simply unzip it. It contains various out-of-the-box examples.  We will be focusing on the jbpm-quarkus-example here.

### Building and running jbpm-quarkus-example

The jbpm-quarkus-example shows how you can build your own order service by leveraging a business process to describe the logic that the service should follow.  The example includes a simple process that describes the steps that need to be followed when ordering items: a sequence of a script task (which is writing out some debug info) and a call activity invoking a sub-process, using a custom `Order` data element.

![My helpful screenshot](/assets/images/get-started/kogito_gettingstarted_graphics_demo-one.png)

The sub-process invokes a custom Java service `CalculationService.calculateTotal`, followed by a user task to verify the order.

![My helpful screenshot](/assets/images/get-started/kogito_gettingstarted_graphics_demo-two.png)

Based on these two processes (defined using BPMN 2.0 format), the custom data object and the custom Java service mentioned earlier, the example shows how a new service is generated that exposes REST operations to create new orders (following the steps as defined in the main and sub-process), or to list and delete active orders. You can choose to create this service based on either Quarkus or SpringBoot.

## Quarkus

Open your command line and go into the jbpm-quarkus-example folder.  First we will build the service.  Based on the process definitions, this will generate the necessary code to turn this into domain-specific order service with REST endpoints to start, list and remove orders.  

For local development, you have 3 options to build and start the service:
* Since the service runs on top of Quarkus, you can take advantage of the development capabilities that Quarkus offers (like live reload etc.), and run the service in Quarkus development mode.
* You can also run the service as a regular Java service.
* You can take advantage of native image compilation (requires GraalVM), which will further optimize and minimize the service using native image compilation.

### Build and run in development mode

`mvn clean package quarkus:dev`

### Build and run in JVM mode

```
mvn clean package 
java -jar target/jbpm-quarkus-example-{version}-runner.jar  
or on Windows
java -jar target\jbpm-quarkus-example-{version}-runner.jar 
```

### Build and run in native mode (requires GraalVM)

```
mvn clean package -Pnative
./target/jbpm-quarkus-example-{version}-runner
```

<div class="orange">Note: This does not yet work on Windows, GraalVM and Quarkus should be rolling out support for Windows soon.</div>

## Spring boot

Open your command line and go into the jbpm-springboot-example folder. First we will build the service.  Based on the process definitions, this will generate the necessary code to turn this into domain-specific order service with REST endpoints to start, list and remove orders.

For local development, you have 2 options to build and start the service:
* Since the service runs on top of SpringBoot, you can take advantage of the development capabilities that SpringBoot offers and run the service using the SpringBoot maven plugin.
* You can also run the service as a regular Java service.

### Build and run in development mode

`mvn clean package spring-boot:run`

### Build and run in JVM mode

```
mvn clean package 
java -jar target/jbpm-springboot-example-{version}.jar  
or on Windows
java -jar target\jbpm-springboot-example-{version}.jar
```

### Test the running service

Once the service is up and running, you can use the following examples to interact with the service.  Below are curl command you can run to do the REST calls but feel free to use the tool of your choice as well.

### POST /orders

Allows to create a new order with the given data:

```
curl -d '{"approver" : "john", "order" : {"orderNumber" : "12345", "shipped" : false}}' -H "Content-Type: application/json" -X POST http://localhost:8080/orders
```

As response the updated order is returned.

### GET /orders

Returns list of orders currently active:

`curl -X GET http://localhost:8080/orders`

As response an array of orders is returned.

### GET /orders/{id}

Returns order with given id (if active):

`curl -X GET http://localhost:8080/orders/1`

As response a single order is returned if found, otherwise no content (204) is returned.

### DELETE /orders/{id}

Cancels order with given id

`curl -X DELETE http://localhost:8080/orders/1`

You can try out other examples as well, all of them are equipped with a Readme file describing how to use them.

## Create your first application

This guide covers
* Configuring your IDE with modeller
* Generating new project
* Building the project
* Testing the project

#### Install Eclipse with modelling plugins

To be able to make use of visual modelling of your processes download Eclipse IDE and install from Marketplace
* Eclipse BPMN2 Modeler plugin (with jBPM Runtime Extension)

<div class="orange">Note: Currently the Eclipse IDE is the only IDE that has complete support for both process and rule modelling but the team is working on bringing in web-based embeddable BPMN2, DMN and Scenario editors to VSCode and Eclipse Che.</div>

To build your own service that is powered by Kogito the best way is to start by generating project using Maven Archetype.

## Quarkus

### Generate project

```
mvn archetype:generate -DarchetypeGroupId=org.kie.kogito -DarchetypeArtifactId=kogito-quarkus-archetype -DarchetypeVersion=0.1.3 -DgroupId=com.company -DartifactId=sample-kogito
```

Once the project is generated, import it into your Eclipse IDE. There is a single process included in the project out-of-the-box that allows to test the generated application. Simply build the project with maven and start the application (as before you have the option to start it using Quarkus dev mode, using JVM mode or using native image mode - we will use Quarkus dev mode in this example)

### Start your application

Open your command line and go into the newly created sample-kogito folder

`mvn clean package quarkus:dev`

## SpringBoot

### Generate project

```
mvn archetype:generate -DarchetypeGroupId=org.kie.kogito -DarchetypeArtifactId=kogito-springboot-archetype -DarchetypeVersion=0.1.3 -DgroupId=com.company -DartifactId=sample-kogito
```

Included in the project out-of-the-box that allows to test the generated application. Simply build the project with maven and start the application (as before you have the option to start it using SpringBoot maven plugin or as a normal Java service - we will use the SpringBoot maven plugin in this example)

### Start your application

Open your command line and go into the newly created sample-kogito folder.

`mvn clean package spring-boot:run`

### Test your application

Once the service is up and running, you can use the following examples to interact with the service.  Below are curl command you can run to do the REST calls but feel free to use the tool of your choice as well.

```
curl -X POST -H 'Content-Type: application/json' -H 'Accept: application/json' -d '{}' http://localhost:8080/tests
```

That gives you a starting point where you can start adding your own business processes, rules and decisions!


















































