---
layout: guides
title: Kogito - Guides
permalink: /guides/
---

<div class="grid__item width-4-12 hide-mobile toc" markdown="1">
## Table of Contents

### Getting started
 - [Kogito business automation overview](https://docs.jboss.org/kogito/release/latest/html_single/#con-kogito-automation_kogito-docs)
 - [Creating and running your first Kogito services](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-creating-running)
 - [Example applications with Kogito services](https://docs.jboss.org/kogito/release/latest/html_single/#ref-kogito-app-examples_kogito-creating-running)
 - [Deploying Kogito services on OpenShift](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-deploying-on-openshift)
 - [Travel agency tutorial for Kogito services on OpenShift](https://docs.jboss.org/kogito/release/latest/html_single/#con-kogito-travel-agency_kogito-deploying-on-openshift)

### Tooling
 - [Kogito BPMN and DMN modelers](https://docs.jboss.org/kogito/release/latest/html_single/#con-kogito-modelers_kogito-creating-running)

### Kogito on OpenShift
 - [Deploying Kogito services on OpenShift](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-deploying-on-openshift)

### Decision services
 - [Developing decision services with Kogito](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-developing-decision-services)
 - [Using DMN models in Kogito services](https://docs.jboss.org/kogito/release/latest/html_single/#_using_dmn_models_in_kogito_services)
 - [Using DRL rules in Kogito services](https://docs.jboss.org/kogito/release/latest/html_single/#_using_drl_rules_in_kogito_services)
 - [Using spreadsheet decision tables in Kogito services](https://docs.jboss.org/kogito/release/latest/html_single/#_using_spreadsheet_decision_tables_in_kogito_services)
 - [Decision engine in Kogito](https://docs.jboss.org/kogito/release/latest/html_single/#_decision_engine_in_kogito)

### Process services
 - [Developing process services with Kogito](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-developing-process-services)
 - [BPMN 2.0 support in Kogito](https://docs.jboss.org/kogito/release/latest/html_single/#con-bpmn_kogito-developing-process-services)
 - [Persistence in Kogito services](https://docs.jboss.org/kogito/release/latest/html_single/#con-persistence_kogito-developing-process-services)
 - [Kogito Management Console](https://docs.jboss.org/kogito/release/latest/html_single/#con-management-console_kogito-developing-process-services)

### Environment configuration
 - [Configuring Kogito supporting services and runtime capabilities](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-configuring)
 - [Using the Kogito Data Index Service](https://docs.jboss.org/kogito/release/latest/html_single/#con-data-index-service_kogito-configuring)
 - [Using the Kogito Jobs Service](https://docs.jboss.org/kogito/release/latest/html_single/#con-jobs-service_kogito-configuring)

</div>
<div class="grid__item width-8-12 width-12-12-m gs-content">

You have gone through the <a href="{{site.baseurl}}/get-started">Getting Started guides</a>. You are now ready to dive into specific topic guides.

<h2 id="Tooling">Tooling</h2>

<div class="guide-item" markdown="1">
### Kogito BPMN and DMN modelers

Kogito provides extensions and application graphical modelers that you can use to design Business Process Model and Notation (BPMN) process models and Decision Model and Notation (DMN) decision models for your Kogito services.

For convenience, all Kogito BPMN and DMN modelers are available in the [Business Modeler Hub desktop application](https://docs.jboss.org/kogito/release/latest/html_single/#proc-kogito-modelers_kogito-creating-running).

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#con-kogito-modelers_kogito-creating-running" class="button-cta secondary">READ THE GUIDE</a>
</div>

<h2 id="Kogito_on_OpenShift">Kogito on OpenShift</h2>

<div class="guide-item" markdown="1">
### Deploying Kogito services on OpenShift

Deploy Kogito services on OpenShift for cloud implementation. In this architecture, Kogito services are deployed as OpenShift pods that you can scale up and down individually to provide as few or as many containers as required for a particular service. You can use standard OpenShift methods to manage the pods and balance the load.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-deploying-on-openshift" class="button-cta secondary">READ THE GUIDE</a>
</div>

<h2 id="Decision_services">Decision services</h2>

<div class="guide-item" markdown="1">
### Developing decision services with Kogito

As a developer of business decisions, you can use Kogito business automation to develop decision services using Decision Model and Notation (DMN) models, Drools Rule Language (DRL) rules, XLS or XLSX spreadsheet decision tables, or a combination of all three methods.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-developing-decision-services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Using DMN models in Kogito services

As a business analyst or business rules developer, you can use Decision Model and Notation (DMN) to model a decision service graphically in a decision requirements diagram (DRD). This diagram consists of one or more decision requirements graphs (DRGs) that trace business decisions from start to finish, with each decision node using logic defined in DMN boxed expressions such as decision tables.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#_using_dmn_models_in_kogito_services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Using DRL rules in Kogito services

As a developer of business decisions, you can define business rules using Drools Rule Language (DRL) directly in free-form .drl text files. A DRL file can contain one or more rules that define at a minimum the rule conditions (when) and actions (then).

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#_using_drl_rules_in_kogito_services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Using spreadsheet decision tables in Kogito services

As a developer of business decisions, you can define business rules in a tabular format in spreadsheet decision tables and then include the spreadsheet file in your Kogito project. These rules are compiled into Drools Rule Language (DRL) for the decision service in your project.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#_using_spreadsheet_decision_tables_in_kogito_services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Decision engine in Kogito

As a developer of business decisions, your understanding of the decision engine in Kogito can help you design more effective business assets and a more scalable decision management architecture. The decision engine is the Kogito component that stores, processes, and evaluates data to execute business rules and to reach the decisions that you define. This document describes basic concepts and functions of the decision engine to consider as you create your business rule system and decision services in Kogito.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#_decision_engine_in_kogito" class="button-cta secondary">READ THE GUIDE    </a>
</div>

<h2 id="Process_services">Process services</h2>

[Developing process services with Kogito](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-developing-process-services)
 - [BPMN 2.0 support in Kogito](https://docs.jboss.org/kogito/release/latest/html_single/#con-bpmn_kogito-developing-process-services)
 - [Persistence in Kogito services](https://docs.jboss.org/kogito/release/latest/html_single/#con-persistence_kogito-developing-process-services)
 - [Kogito Management Console](https://docs.jboss.org/kogito/release/latest/html_single/#con-management-console_kogito-developing-process-services)

<div class="guide-item" markdown="1">
### Developing process services with Kogito

As a developer of business processes, you can use Kogito business automation to develop process services using Business Process Model and Notation (BPMN) 2.0 models. BPMN process models are graphical representations of the steps required to achieve a business goal. You can design your BPMN processes with the Kogito BPMN modeler in VSCode or import existing BPMN processes into your Kogito projects for deployment and execution.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-developing-process-services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### BPMN 2.0 support in Kogito

Business Process Model and Notation (BPMN) 2.0 is a standard established by the Object Management Group (OMG) for describing and modeling business processes.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#con-bpmn_kogito-developing-process-services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Persistence in Kogito services

Kogito supports runtime persistence for preserving process data in your services across application restarts. Kogito persistence is based on key-value storage to persist data, such as active process nodes and process instance variables.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#con-persistence_kogito-developing-process-services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Kogito Management Console

The Kogito Management Console is a user interface for viewing the state of all available Kogito services and managing process instances. You can use the Management Console to view process, subprocess, and node instance details, abort process instances, and view domain-specific process data.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#con-management-console_kogito-developing-process-services" class="button-cta secondary">READ THE GUIDE</a>
</div>

<h2 id="Environment_configuration">Environment configuration</h2>
 - [Configuring Kogito supporting services and runtime capabilities](https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-configuring)
 - [Using the Kogito Data Index Service](https://docs.jboss.org/kogito/release/latest/html_single/#con-data-index-service_kogito-configuring)
 - [Using the Kogito Jobs Service](https://docs.jboss.org/kogito/release/latest/html_single/#con-jobs-service_kogito-configuring)

<div class="guide-item" markdown="1">
### Configuring Kogito supporting services and runtime capabilities

As a developer of business processes and decisions, you can configure Kogito supporting services and runtime properties for advanced use cases with your Kogito services.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#chap-kogito-configuring" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Using the Kogito Data Index Service

Kogito provides a Data Index Service that stores all Kogito events related to processes, tasks, and domain data. The Data Index Service is at the core of all Kogito search, insight, and management capabilities.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#con-data-index-service_kogito-configuring" class="button-cta secondary">READ THE GUIDE</a>
</div>

<div class="guide-item" markdown="1">
### Using the Kogito Jobs Service

Kogito provides a Jobs Service for scheduling Business Process Model and Notation (BPMN) process events that are configured to be executed at a specified time. These time-based events in a process model are known as jobs.

<a href="https://docs.jboss.org/kogito/release/latest/html_single/#con-jobs-service_kogito-configuring" class="button-cta secondary">READ THE GUIDE</a>
</div>

</div>
