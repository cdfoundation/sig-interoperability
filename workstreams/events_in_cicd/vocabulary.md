# CD Events Vocabulary Proposal

This document intends to describe a set of events related to different phases of a Continuous Delivery process. 
These events are categorized by meaning and the phase where they are intenteded to be used. 
These events are agnostic from any specific tool and are designed to fit a wide range of scenarios. 

The phases covered by this proposal are:

- **Source Code Version Control Events**: Events emitted by changes in source code or by the creation, modification or deletion of new repositories that hold source code.
- **Continuous Integration Pipelines Events**: includes events related to building, testings, packaging and releasing software artifacts, usually binaries.
- **Continuous Deployment Pipelines Events**: include events related with environments where the artifacts produced by the integration pipelines actually run. These are usually services running in a specific environment (dev, QA, production), or embeded software running in a specific hardware. 


# Required Metadata for CD Events

The following attributes are REQUIRED to be present in all the Events defined in this vocabulary:

- **Event ID**: defines a unique identifier for the event
- **Event Type**: defines a textual description of the event type, only event types described in this document are supported
- **Event Source**: defines the context in which an event happened
- **Event Timestamp**: defines the time when the event was produced

The following sections list the events in different phases, allowing adopters to choose the events that they are more interested in.

# Source Code Version Control Events

This phase includes events related to changes in Source Code repositories that are relevant from a Continuous Delivery perspective.


## Repository Events

These events are related to Source Code repositories
- **Repository Created Event**: a new Source Code Repository was created to host source code for a project
- **Repository Modified Event**: a Source Code Repository modified some of its attributes, like location, or owner
- **Repository Deleted Event**: a Source Code Repository was deleted and it is not longer available
- **Branch Created Event**: a Branch inside the Repository was created 
- **Branch Deleted Event**: a Branch inside the Repository was deleted
- **Change Committed**: a change is commited to a branch
- **Change Approved**: a change request is created by a user, that requires review and approval before being applied to an existing branch inside the repository
- **Change Rejected**: a change was reviewed and rejected by a user
- **Change Merged**: a change request has been merged to a branch in an existing repository



# Continuous Integration Pipeline Events

These events are related to continuous integration pipelines, this pipelines usually include building, testing, packaging and releasing software artifacts. 
Due the dynamic nature of Pipelines, most of actual work needs to be queued to happen in a distributed way, hence Queued events are added. 
Adopters can choose to ignore these events if they don't apply to their use cases. 

- **Pipeline Queued**: a Pipeline has been schedule to start
- **Pipeline Started**: a Pipeline has started
- **Pipeline Finished**: a Pipeline has finished, the event will contain the finished status, success, error or failure
- **Build Queued**: a Build task has been queued, this build process usually is in charge of producing a binary from source code
- **Build Started**: a Build task has started 
- **Build Finished**: a Build task has finished, the event will contain the finished status, success, error or failure
- **Tests Started**: a Test task has started
- **Tests Finished**: a Test task has finished, the event will contain the finished status, success, error or failure
- **Artifact Packaged**: an artifact has been packaged for distribution, this artifact is now versioned with a fixed version
- **Artifact Released**: an artifact has been released and it can be advertised for others to use


# Continuous Deployment Pipelines Events 

These events are related to continous deployment pipelines and their target environments. 
These events can be emitted by environments to report where software artifacts such as services, binaries, deamons, jobs or embeded software are running. 

The term Service is used to represent a running Artifact. This service can represent a binary that is running, a deamon, an application, a docker container, etc.
The term Environment represent any platform which has all the means to run a Service. 

- **Environment Created**: an environment has been created and it can be used to deploy Services
- **Environment Modified**: an environment has been modified, this event advertise the changes made in the environment
- **Environment Deleted**: an environment has been deleted and cannot longer be used
- **Service Deployed**: a new instance of the Service has been deployed
- **Service Upgraded**: an existing instance of a Service has been upgraded to a new version
- **Service Undeployed**: an existing instance of a Service has been terminated an it is not longer present in an environment
