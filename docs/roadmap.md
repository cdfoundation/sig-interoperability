# CDF SIG Interoperability Roadmap

## Quick Links

- [Overview](#overview)
- [Charter](#charter)
- [Outcomes](#outcomes)
- [Roadmap](#roadmap)
- [Contributors](#contributors)

## Overview

This document outlines the roadmap for the Continuous Delivery Foundation (CDF)
Interoperability Special Interest Group (SIG). The roadmap represents the
initiatives of the open source collaborations. The roadmap does not specify
timelines or delivery dates, but rather uses time horizons (now, next, later).

## Charter

The CDF Interoperability SIG works to solve the problems of making CI/CD
software tools interoperable and interchangeable. 

Software interoperability is essential to drive CI/CD tool adoption as well as
promote innovation in the industry. To achieve this, the SIG will strive to
collaboratively develop and expedite well defined definitions, interfaces, and
reusable software libraries, services and applications. 

## Outcomes 

The group will work towards a number of outcomes 

1. **Knowledge Transfer of CI/CD Tools & Technologies:** We share information
   about open source CI/CD tools, infrastructure and frameworks.
2. **End User Requirements:** We capture actual ways end users are using tools,
   the problems they are trying to solve, the pain points they are experiencing
   particularly around tool integration. 
3. **Shared Reference Terminology:** We work on establishing shared vocabulary
   since CI/CD practitioners have many tools and technologies at their disposal
   but it is often the case that what we call a pipeline in today’s tool of
   choice is not called the same thing in the tool we use tomorrow. 
4. **Interoperable Tools:** It is almost always the case that the CI/CD systems
   organizations employ evolve continuously, new tools are brought in and others
   phased out, making it crucial for users to have tool interoperability in
   order to ease the effort to get the best out of the systems and establish
   end-to-end flow of software with the help of well-defined interfaces,
   reusable libraries, services, and applications.
5. **Standardized Frameworks**
6. **Promote Best Practices**

## RoadMap

![](https://lh5.googleusercontent.com/5F-b4dHm1MMqn47PNzMx9Br7h6N62fEnZU3xp60E9LksEo-MmOK8Ok0PqjyAet4oevSk4vXcgfdi7wg8V4gRuvklCDoO57km-r6DKZS7w4IFhlquyq4_KCHrcYVZNXR1EIRTyDxO)

Reference: Janna Bastow (https://twitter.com/simplybastow/status/1168531737766432768?s=20)


### Completed

#### Knowledge transfer of CI/CD Tools and Technologies
    
The CDF SIG holds regular presentations to enable knowledge sharing about CI/CD
Tools & Technologies, infrastructure, and frameworks.

Presentations of the following tools and technologies are completed.

* [Tekton](https://tekton.dev/)
* [Keptn](https://keptn.sh/)
* [Zuul](https://zuul-ci.org/)
* [Eiffel](https://eiffel-community.github.io/)
* [Jenkins X](https://jenkins-x.io/)
* [Flagger](https://flagger.app/)
* [Tekton Catalog and Hub](https://tekton.dev/)
* [Argo Rollouts](https://argoproj.github.io/argo-rollouts/)

#### Documenting and Publishing CI/CD Vocabulary

The vocabulary/terminology used by various CI/CD tools & technologies have been
documented in [SIG Interoperability repository](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/vocabulary.md)
and an article is contributed to [CDF Newsletter](https://cd.foundation/blog/2020/04/24/how-the-cdf-is-establishing-a-shared-vocabulary-for-the-industry/).

### Now 

#### Knowledge transfer of CI/CD Tools and Technologies

The CDF SIG will continue working on knowledge transfer of CI/CD Tools and
Technologies in order to identify trends and explore further cross community
collaboration opportunities.

Upcoming presentations include

* Jenkinsfile Runner
* Spinnaker
* Lighthouse

#### End User Case Studies

End users will share use cases, challenges, and the work they are doing within
their organizations with the community in order to enable dialog and further
collaboration.

* eBay

#### Identify Focus Areas

Interoperability in CI/CD tools and technologies means different things to
different people depending on the activities they are performing in their CI/CD
workflows, tools and technologies they are using, integration points they may
have within their systems and so on. Some examples to this are

* An organization employing more than one technology to establish and run CI/CD
  pipelines due to different capabilities provided by the tools and the
  organization wants to have means to construct these pipelines in a
  standardized way
* An organization with multiple subunits where different components are
  developed and delivered needs to have ways to connect the CI/CD pipelines
  constructed using different tools within sub-units in a standardized way to
  establish end to end traceability
* An organization with CI/CD workflows spanning across multiple units, internal
  and/or external, wants to visualize what is going on within CI/CD workflow any
  point in time and in a real time or historical manner
* An organization with the aim to actively engage with its customers in the
  product lifecycle and receive continuous feedback from their integration and
  delivery flows.
* An organization with CI/CD system would like to migrate to different set of
  tools without developing new pipelines from scratch
* An organization that want to integrate other tools such as Software
  Configuration Management Systems (SCM), Artifact Repository Managers (ARM),
  and so on with CI/CD tools they are using in a ways that is agnostic to SCM,
  ARM, and CI/CD tools they are using so they can abstract the logic away from
  the tools and focus on software flow

As it can be seen from the examples above, there are different needs that need
to be addressed. Tackling these in a more structured manner would make it easier
to get the collaboration going. To enable this, the SIG started identifying few
focus areas based on the conversations happening within the SIG.

Some of the identified areas are

* **Events in CI/CD**: Events are everywhere and new tools and technologies,
  including the ones within CI/CD domain, already adapted this such as
  [Tekton](https://github.com/tektoncd/triggers), [Keptn](https://keptn.sh/),
  and [Eiffel](https://eiffel-community.github.io/). 
* **Reusable Libraries**: There are various libraries that are developed by
  different communities such as [go-scm](https://discourse.drone.io/t/go-scm-jenkins-x-tekton-and-cdf/6698).
  SIG and CDF could provide home for collaboration on reusable libraries,
  helping with further development, coordination, and sharing of them.

#### Establish Workstreams

The way the SIG could enable further collaboration and focused work on the
areas is identified as introducing workstreams within the SIG, each working
on a specific area. The project and user representatives who take part in the
SIG can volunteer as workstream lead or contributor and work on the areas in a
more focused and structured way, continuously sharing the progress with the rest
of the SIG. The expectations from workstreams could vary depending on the area;
they could work on collecting the state of things in a specific area from within
the ecosystem and contribute that to the domain or come up with a proposal to
address some of the needs in a more structured way in order to socialize their
ideas further and increase the awareness. This could also help us to present
ideas per area on CDF TOC level in order to gather feedback.

The process around establishing, running, and retiring SIG workstreams is
currently being documented in [SIG Interoperability repository](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/workstream-governance.md).

### Next

#### Establishing Shared Terminology

SIG Vocabulary document, "The Rosetta Stone", makes it possible for the CI/CD
ecosystem to collect and share the terminology used by different CI/CD tools
and technologies in one place, making it easier for the community to see the
commonalities and differences.

The Rosetta Stone could be seen as the basis for getting the dialog going about
the benefits of establishing (defacto) terminology for CI/CD domain and
drive the standardization within interoperability further.

Possible steps to achieve this goal are

* Include additional tools and technologies within the document (12 CI/CD tools
  and technologies are included in the document)
* Continue highlighting this work and get help from others to increase the
  participation
* Demonstrate the benefits clearly
* Stress the importance of doing this work in a real neutral place where
  project and user representatives could take part
* Prioritize things that matter (interoperability is more key than common
  language)
* Establish process around how to start and drive the work on standardization
* Establish de facto terms 

Some of the challenges we foresee are

* Friction for maintainers to change terminologies and whether we can
  simplify this
* Companies will have own internal (proprietary) tools and terminology

#### Additional Focus Areas

In addition to the focus areas SIG identified and started working, various
other areas are also highlighted as potential areas to work.

* **Pipeline Data for Traceability and Visualization**: How can we propagate
  data from our CI/CD tools in a way that external tools can consume it
  regardless of what CI/CD tool created the data? 
* **Pipeline standardization/languages**

* **Integration with the tools that are not traditionally seen as CI/CD tools**

#### Standardized Frameworks

As a preparation for defining interfaces, libraries and services, first we must
collect, discuss, and build an understanding of common tasks solved in CI/CD
workflows. This list would contain tasks as listed below.

* **Merge source code**: This task is typically not performed by the CI/CD
  pipelines themselves, unless automatic baseline uplifts are performed in
  those systems, but it serves as the trigger for the CI pipeline/workflow.
* **Source code tests**: Typically Lint tests or other static code analysis
  done before building the source code.
* **Build**: Producing artifacts from the source code. Potentially including
  other source code repositories, libraries and pre-built artifacts from other
  sources.
* **Binary tests**: Testing the built binary. In a Kubernetes environment this
  is normally done after the deployment step below, but in VMs and legacy
  environments this is typically done as the first thing after the build.
* **Configuration change**: The availability of a new software artifact or a new
  configuration (e.g. changed environment variables, arguments, etc.) lead to a
  configuration change. This configuration change is the trigger for a CD
  workflow. In a GitOps approach, this configuration change could be a commit or
  a Pull Request.
* **Pre-deployment**: Before doing the actual deployment, some environments
  first need to be prepared. A common use case would be to run DB migration
  scripts.
* **Deployment**: Run the new configuration in your environment (pre-prod, prod).
  This resulting new service can either replace an old version of the same service
  or can run next to old versions (e.g. for B/G deployments). After doing the
  deployment, the new service is not necessarily exposed to actual users, i.e.
  the service does not serve production traffic.
* **Test**: Perform all different kinds of tests like smoke tests, dark tests,
  security tests, integration tests, end-to-end tests, etc.
* **Verification/Validation/Evaluation**: Automatically validate the performance
  of the new service using quality gates based on e.g. Service Level Indicators
  (SLIs) and Service Level Objects (SLOs). Keywords: “Quality Gates”,
  “Progressive Delivery”
* **Approval**: Engineers manually approve the new service.
* **Release**: Routes real user traffic to the new service (i.e. canary
  release).
* **Release Verification/Validation/Evaluation**: During the rollout, check for
  any problems using e.g. monitoring data.
* **Rollback**: This task is optionally executed if the new version does not
  perform well.
* **Clean up**: Stop old versions of the service, which are not needed anymore.
* **Continuous feedback**: At least in a devops context, there could be systems
  continuously monitoring the deployments running in production and providing
  feedback back to the product developers

Overall, a collection of these tasks could direct us to the points where interfaces and libraries are needed.

### Later

#### Events Standardizations

## Contributors  

The work with the roadmap was started by Tracy Miranda and the draft version
of this document was developed on [Google Docs](https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit#).

This version is the result of many discussions that took place during SIG
meetings and many iterations and discussions that took place
during SIG meetings. The contributors listed below made valuable contributions
to the roadmap by either taking part in discussions, sharing their thoughts
on the document, and/or editing the roadmap directly.

Please note that the list of contributors are listed alphabetically.

* Andreas Grimmer
* Christie Wilson
* Emil Bäckmark
* Emelie Pettersson
* Eric Sorenson
* Fatih Degirmenci
* Ignacio Pascual
* Kara de la Marck
* Ramin Akhbari
* Tracy Miranda
