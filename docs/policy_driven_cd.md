# Policy Driven CD

## Quick links

* [Introduction](#Introduction)
* [Policy Types](#Policy-Types)
* [Open Source Policy Frameworks](#Open-Source-Policy-Frameworks)
    * [Open Policy Agent](#Open-Policy-Agent)
    * [ONAP Policy Framework](#ONAP-Policy-Framework)
* [Approaches to Policy](#Approaches-to-Policy)
    * [Communities](#Communities)
        * [Jenkins](#Jenkins)
        * [Spinnaker](#Spinnaker)
        * [Tekton](#Tekton)
        * [Ortelius](#Ortelius)
        * [DeployHub Pro](#DeployHub-Pro)
        * [Zuul](#Zuul)
    * [Users](#Users)
        * [eBay](#eBay)
        * [Ericsson](#Ericsson)
* [Challenges](#Challenges)
    * [Terminology](#Terminology)
    * [Best Practices](#Best-Practices)
    * [Interoperability](#Interoperability)
* [References](#References)

## Introduction

TBD

## Policy Types

TBD

## Open Source Policy Frameworks

### Open Policy Agent

Open Policy Agent is an infrastructure agnostic policy engine with the mission of decoupling decisions
about policy from other application business logic, via "policies as code".

Policies are expressed in a language called Rego which is supported via:

* An online playground: https://play.openpolicyagent.org/
* IDE integrations (e.g. [vscode](https://marketplace.visualstudio.com/items?itemName=tsandall.opa))
* [Testing capabilities](https://www.openpolicyagent.org/docs/latest/policy-testing/)
* [Command line REPL](https://www.openpolicyagent.org/docs/latest/#2-try-opa-eval)

### ONAP Policy Framework

TBD

## Approaches to Policy

### Communities

#### Jenkins

TBD

#### Spinnaker

TBD

* The Armory flavor of Spinnaker [supports OPA](https://docs.armory.io/docs/armory-admin/policy-engine-enable/)

#### Tekton

A few ways that Tekton could integrate with Policy frameworks:

* Enforcing policies via kubernetes webhooks (e.g. looking at TaskRuns and PipelineRuns),
  and either:
  * Preventing them from executing when policies are violated
  * Mutating them to enforce policies
* Using policies to generate Pipelines and Tasks (e.g. express CD pipelines completely
  via policy)
* Using [when expressions](https://github.com/tektoncd/pipeline/blob/master/docs/pipelines.md#guard-task-execution-using-whenexpressions)
  as gates to control execution of Tasks in a Pipeline
* [Tekton Chains](https://github.com/tektoncd/chains) has a goal to store trusted
  information about executions and policies could be expressed against this
* Tekton Triggers has support for [interceptors](https://github.com/tektoncd/triggers/blob/master/docs/eventlisteners.md#interceptors)
  for filtering, with built in support for CEL and extensibility which could support
  [Rego](https://github.com/tektoncd/triggers/issues/484)
  
An interesting question to answer about policy is do you want it to be _reactive_ or
_proactive_, e.g. do you want to find out that you are violating a policy, or do you
want to use a policy to decide what you do.

#### Ortelius
Ortelius, serving as a centralized catalog for microservice deployment metadata and relationships is relatively unrestricted with some built-in guardrails.

* License policy would ensure all components for an application version conform to an approved list of licenses.  Ortelius would enforce that application versions from consuming components with unapproved licenses would not be deployed.

* CVE policy would ensure all components for an application version conform to a risk level.  Ortelius would enforce that application versions consuming components with a high risk level would not be deployed.

* Configuration policy would be used to ensure specific configurations are in place for the application versions, component versions and environment combination. 
  
  For example, does the cluster have enough nodes in it.
  
  Ortelius would enforce that the configuration is in conformance and prevent the application version from being deployed if there is a policy violation.

#### DeployHub Pro

A few ways that DeployHub Pro could integrate with Policy frameworks:

* Authorization policy would be used to validate who can do what preventing unauthorized actions from happening.

  For example, which users can update a component or which group can execute a deployment. 
  
* Approved Component policy would be used to ensure all components for an application are on the "Approved to Use" list.  This policy would allow new unapproved components in development but restricted for testing and production. DeployHub Pro would enforce the consumption of the components by applying the appropriate policy for the pipeline stage (dev, test, prod).

* License policy would ensure all components for an application version conform to an approved list of licenses.  DeployHub Pro would enforce that application versions from consuming components with unapproved licenses would not be deployed.

* CVE policy would ensure all components for an application version conform to a risk level.  DeployHub Pro would enforce that application versions consuming components with a high risk level would not be deployed.

* Duplicate Component policy would be used to minimize the copying of code instead of it being made available as reusable code.  DeployHub Pro would enforce that application versions consuming components do not have copied code in a component and would prevent the application version from being deployed.

* SLO/SLI policy would be used as a reactive policy to revert a deployment to its previous version if the policy has been violated.  DeployHub Pro would redeploy the previous version of the application to the environment.

* Configuration policy would be used to ensure specific configurations are in place for the application versions, component versions and environment combination. 
  
  For example, does the cluster have enough nodes in it.
  
  DeployHub Pro would enforce that the configuration is in conformance and prevent the application version from being deployed if there is a policy violation.

#### Zuul

Zuul's configuration covers job definitions and mapping them to build triggers with project pipelines. Because this configuration can be distributed across any of the Git repositories it knows about (even speculatively consuming configuration from proposed changes not yet merged), the people who control the content of those repositories or who can propose changes for them.
The system has particular means of centralizing configuration so the operators control certain aspects.
Zuul has trusted configuration repositories which could mean that specific jobs are run on specific events and these jobs are immutable.



### Users

#### eBay

The approach to policy at eBay is more of a badge system. Badges are awarded by a central authority and events are produced based on this so other systems could subscribe to them.
We are trying to make sure that as the manifest for a particular release is moving from environment to environment with ultimate goals to reach production.
They achieve certain things along the way - those things are making sure a project or an application has a CD pipeline defined (build/unit tests/integration tests/security tests).
All of these basically become badges so a manifest of an application that's a candidate for release receives along the way.
For example; when unit tests finish, they report back to system and the system takes the manifest id, awarding a badge and so on and so forth.
When they are ready to deploy to staging environment, it requires manifests to have certain set of badges to in order to be deployed.
Otherwise, deployment is denied.
This ensures things are done as per the company policy for different environments. (feature environment, staging environment, pre-production environment, production environment)

This is similar to gating - gate allows or prevents deployment of a certain environments based on badges.

#### Ericsson

The use case at Ericsson is pretty similar to eBay.
At Ericsson, the term " "Confidence Levels" are used. These confidence levels are applied when an artifact passes certain type of tests, gaining confidence levels. These confidence levels are carried by events, triggering actual deployments.
In this case, the "Deployment system" doesn't search for badges but events are the main medium to trigger stuff.

## Challenges

### Terminology

eBay: Badges are used to enforce policies  
Ericsson: Confidence Levels are used to enforce policies

### Best Practices

TBD

### Interoperability

TBD

## References

TBD