---
layout: trustyai
title: TrustyAI
permalink: /trustyai/
---

# TrustyAI Initiative
<br/>

The TrustyAI initiative aims to offer value-added services to the Kogito ecosystem to make it a trustworthy Business Automation solution. The project currently focuses on the open DMN standard and introspects the decision-making process using the following aspects:

- **Explainability**: Enrich model execution information through XAI algorithms
- **Tracing and Accountability**: Extract, collect, and publish metadata for auditing and compliance
- **Runtime Monitoring**: Expose services in dashboards to assess data from both a business and an operational perspective

## Value-added services

### Explanability
TrustyAI aims to help explain black-box machine learning models by using XAI techniques. 
Black-box models are not transparent about their processing, and the user only knows the inputs and outcomes of the system. 
An example of this is a neural network: These models are accurate for predictions, but their complexity can make them hard to interpret. 

XAI techniques are used within TrustyAI to introspect these black-box models to describe predictions and outcomes. 
This is done by looking at a feature importance chart. This is where the model’s inputs are ordered by the most important ones for the decision-making process. 
This can help to capture if a model is biased. Model bias can damage a company’s reputation. 
For example, if you have a hiring machine learning system and the most important feature they looked at was gender, this would show a bias. 
TrustyAI reduces the chance of this by showing the important features used in the machine learning model to reduce business risk.

### Tracing and Accountability
The Audit UI is a dashboard that targets business users or auditors, where each transaction is stored and can be analysed. 
For each transaction, it is possible to access the user inputs, the outcomes produced, and the explanation of each of them. 

The Audit UI traces every decision made and helps to create accountability of the system. 
Accountability is guaranteed by the caseworker who can access the outcomes from the decision. 
This means they can ensure that the outcomes of the system meet the requirements of the company.

### Runtime Monitoring
Runtime monitoring allows for both business and operational metrics to be displayed in a Grafana dashboard configurable by the user. 
Business monitoring dashboards are generated based on model information (DMN or machine learning models) so that users can monitor business aspects and have an aggregated view of decision behaviors. 
Finally, operational aspects can be monitored to keep track of the health of the services.


## Contributing

The source code is hosted on GitHub as part of Kogito repositories. If you need to report a bug or request a new feature, look for a similar one on our [Jira issue tracker](https://issues.jboss.org/projects/KOGITO). If you don’t find any, create a new issue.

For suggested bug fixes or improvements specific to the Explainability aspect, you can also use the [research FAI Jira project](https://issues.jboss.org/projects/FAI).

### Chat

Join our community chat by joining the [#trusty-ai](https://kie.zulipchat.com/#narrow/stream/232681-trusty-ai) channel on [https://kie.zulipchat.com/](https://kie.zulipchat.com/).

## Resources

All TrustyAI services are integrated with the Kogito platform and documented as part of the [Kogito documentation](https://docs.jboss.org/kogito/release/latest/html_single/).

### Videos

- [Explanation by Example: the OptaPlanner way](https://youtu.be/4H3U6xyCgMI) (OptaPlanner Week) - Daniele Zonca, Rui Vieira and Tommaso Teofili
- [Can you trust your AI?](https://youtu.be/HdEwp2RhG7w) (KIE Live 13) - Daniele Zonca
- [How to integrate your Kogito application with TrustyAI - Part 1](https://youtu.be/exbOCrq8gJE) - Jacopo Rota
- [How to integrate your Kogito application with TrustyAI - Part 2](https://youtu.be/DtY5aWSYWfU) - Jacopo Rota
- [How to integrate your Kogito application with TrustyAI - Part 3](https://youtu.be/8xoqDerWY2s) - Jacopo Rota

### Blog

You can find more details about what is going on in the [TrustyAI blogposts](https://blog.kie.org/all?s=trusty) on the [KIE blog](https://blog.kie.org/).

### Papers

A detailed analysis of TrustyAI's explainability techniques is available in the [TrustyAI Explainability Toolkit](https://arxiv.org/abs/2104.12717) pre-print.
