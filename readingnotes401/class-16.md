# Serverless Functions

## What is Serverless?

Serverless means that you are not responsible for managing or provisioning the server.  As a dev, we are more focused on writing code. It is a cloud computing application development and execution model.

## How it started

Bare Metal: you were responsible for installing OS, patching etc to make environment that you were deploying your code on.

Virtual Machines: Developers were still responsible for setting up environment, however, the idle times were better with better resource management that was built in.

Containers: We package application code and all the dependencies on a single container which can run on any underlying infrastructure.  For larger apps, this could run into problems with the need for multiple containers.

Serverless: This is the stage we are at now where the developer is only focused on writing code since the infrastructure if built and managed remotely by another source.

## How does it work?

FaaS: Functions as a Service platform. It is provided by the cloud service provider now. They include functions run by events in EDA (event driven architecture).  One of the issues with this is latency issues with timeouts.

Serverless databases, such as SQL and noSQL, and particularly object sotrage are the data layer. Event streaming and messaging are well suited processing workloads, most notably Apache Kafka an event streaming platform. API gateways act as the proxies to web actions and provide: HTTP method routing, client ID and secrets, rate limits, CORS, viewing API usage, viewing response logs, and API sharing policies.

## Benefits of using it

You pay for execution only: there is no idle time.
Auto scalable: taken care of by provider, you are not provisioning for it so you are less concerned with the resources in it.
Faster time to market: Since you aren’t responsible for the environment and provisioning, you can focus solely on the code and get it out to market sooner.
Polyglot Environment: allows you to write in multiple languages since they support multiple languages.  You can write it in the language you are comfortable with.
Highly Available: cloud provider takes care of all the fault tolerance.

## Things I want to know more about

I would like to know which serverless container is most proferred to be used. Specifically, Kubernetes can't run serverless apps without specialized software that integrates it with the cloud platform. I wonder if as time goes on, it may have more of those dependencies of sorts built in.

### Resources

[What is serverless? - Reading](https://www.ibm.com/cloud/learn/serverless#toc-what-is-se-K3xZyJmF)
[What is serverless? - Video](https://www.youtube.com/watch?v=vxJobGtqKVM)

### Links

- >[Advanced Software Development](README.md)
