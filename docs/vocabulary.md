# Establishing Shared Vocabulary

- [Introduction](#introduction)
- [Terminology Used by CI/CD Tools and Technologies](#terminology-used-by-cicd-tools-and-technologies)
  - [ArgoCD](#argo-cd)
  - [CircleCI](#circleci)
  - [Eiffel](#eiffel)
  - [GitHub Actions](#github-actions)
  - [GitLab CI/CD](#gitlab-cicd)
  - [Harness](#harness)
  - [Jenkins](#jenkins)
  - [Jenkins X](#jenkins-x)
  - [Keptn](#Keptn)
  - [Screwdriver](#screwdriver)
  - [Spinnaker](#spinnaker)
  - [Tekton](#tekton)
  - [Zuul](#zuul)
- [Terminology Used by SCM Tools and Technologies](#terminology-used-by-scm-tools-and-technologies)
  - [Gerrit](#gerrit)
  - [GitHub](#github)
  - [GitLab](#gitlab)
- [Mapping of Terms](#mapping-of-terms)
  - [CI/CD Tools and Technologies](#mapping-cicd)
  - [SCM Tools and Technologies](#mapping-scm)
- [Shared Vocabulary](#shared-vocabulary)

## Introduction

There are many ways to greet someone and as humans if we do not understand the
word being used we have the ability to observe body language, process tone,
and even touch. These many different natural inputs allow us as humans to
establish shared vocabulary upon which we have been able to build successful
components relevant to our way of living and social norms of interacting.

Unfortunately for machines, this process is not so easy as we humans have to
decide if we want to establish norms which we often surface when talking about
machine interactions as protocols and best practices or requirements.

Continuous Integration (CI) and Continuous Delivery (CD)  practitioners have
many tools at their disposal but it is often the case that what we call a
pipeline in today’s tool of choice is not called the same thing in the tool we
use tomorrow. Again, we can within our sphere of influence and interaction
adjust for these nuances but machines talking to one another do not have that
same luxury necessarily.

The purpose of this document is to collect the basic terms used by CI/CD tools
and technologies in order to work on establishing a shared vocabulary for us
humans to communicate and collaborate better.

## Terminology Used by CI/CD Tools and Technologies

This section contains list of some key terms used by various CI/CD tools and
technologies.

### ArgoCD

[ArgoCD](https://argoproj.github.io/argo-cd/) is a declarative, GitOps continuous delivery tool for Kubernetes.

Some of the core ArgoCD concept are listed below: [[16]]

- **Application**: A group of Kubernetes resources as defined by a manifest. This is a Custom Resource Definition (CRD).
- **Application controller** [[19]]: Kubernetes controller which continuously monitors running applications and compares live vs. desired state.
- **Application source type**: Which Tool is used to build the application.
- **Target state**: The desired state of an application, as represented by files in a Git repository.
- **Live state**: The live state of that application. What pods etc are deployed.
- **Sync status**: Whether or not the live state matches the target state. Is the deployed application the same as Git says it should be?
- **Sync**: The process of making an application move to its target state. E.g. by applying changes to a Kubernetes cluster.
- **Sync operation status**: Whether or not a sync succeeded.
- **Refresh**: Compare the latest code in Git with the live state. Figure out what is different.
- **Health**: The health of the application, is it running correctly? Can it serve requests?
- **Tool**: A tool to create manifests from a directory of files. E.g. Kustomize or Ksonnet. See Application Source Type.
- **Configuration management tool**: See Tool.
- **Configuration management plugin**: A custom tool.
- **Project** [[17]]: A logical grouping of applications. They enable control over deployment permissions based on source, target and kind, among other criteria.
- **Sync phases** [[18]]: Pre-sync, sync and post-sync allow for controlled orchestrated execution of sync operations.
- **Sync waves**: Within any one sync phase, an additional control of sequential execution is accomplished using waves, to ensure certain resources are healthy before subsequent resources are synced.

### CircleCI

[CircleCI](https://circleci.com) allows teams to rapidly build quality
projects, at scale.

Some of the core CircleCI terms are listed below. [[1]]

- **Step**: A step is a collection of executable commands.
- **Job**: A job is a collection of steps.
- **Workflow**: A Workflow is a set of rules for defining a collection of
jobs and their run order. (used interchangeably with pipeline)
- **Pipeline**: A pipeline is an object that you may configure and run on
the CircleCI platform.
- **Executor**: Defines the underlying technology to run a job.

### Eiffel

[Eiffel](https://eiffel-community.github.io/) is a technology agnostic CI/CD event protocol. The events and their parameters are generic enough to cover any kind of CI/CD engine/framework and SCMs.

Some of the terms used in Eiffel events are listed below. [[14]]

- **Activity**: An activity is any kind of action in a CI/CD system, normally triggered by an operation done in an SCM system or by a previous activity. Activities are hierarchical. Activities could be whole pipelines, pipeline steps or any level of pipeline sub steps.
- **Event**: An Eiffel event is a broadcast notification telling any consumer about an event occurring in the CI/CD pipeline.
- **Artifact**: Artifacts are items or software packages generated in a CI/CD pipeline, for example a built binary or a Docker image. An artifact should be possible to identify using a purl ([package URL](https://github.com/package-url/purl-spec)). An artifact is often the subject of a test executed or a delivery performed within a CI/CD pipeline.
- **Environment**: An Eiffel environment defines the environment in which an activity is executed. Could be for example a host, node, service name/uri, a Docker image or some other kind of machine configuration definition.
- **Source Change**: A source change is the unit of a review. It results in a single commit when merged to the Git repository.
- **Submit**: A submit is the action of merging a source change to its intended target branch.
- *Pipeline*: A pipeline is not a term defined by Eiffel, but it is used in the Eiffel protocol documentation when explaining how Eiffel events can be combined to form a chain of activities often triggered by a source change being created or submitted.
- *Step*: A step is not a term defined by Eiffel, but it is used in the Eiffel protocol documentation to exemplify activities executed in a pipeline.

### GitHub Actions

[GitHub Actions](https://help.github.com/en/actions) enables the creation of
custom software development life cycle (SDLC) workflows using GitHub
repositories.

Some of the core GitHub Actions terms are listed below. [[2]]

- **Action**: Individual tasks that you combine as steps to create a job.
Actions are the smallest portable building block of a workflow.
- **Step**: A step is a set of tasks performed by a job.
- **Job**: A defined task made up of steps.
- **Workflow**: Workflows are made up of one or more jobs and can be scheduled
or activated by an event.
- **Workflow run**: An instance of your workflow that runs when the pre
configured event occurs.
- **Event**: A specific activity that triggers a workflow run.
- **Runner**: Any machine with the GitHub Actions runner application installed.

### GitLab CI/CD

[GitLab CI/CD](https://docs.gitlab.com/ee/ci/introduction/) is a powerful tool
built into GitLab that allows users to apply all the continuous methods
(Continuous Integration, Delivery, and Deployment) to their software with no
third-party application or integration needed.

Some of the core GitLab CI/CD terms are listed below. [[3]]

- **Job**: Instructions that a runner has to execute.
- **Stage**: Elements to group and run jobs in certain way - jobs in same
stage are run in parallel and jobs in next stage run after the jobs from the
previous stage completed successfully.
- **Pipeline**: A collection of jobs split into different stages.
- **Runner**: An agent or server that executes each job individually that can
spin up or down as needed.
- **Trigger**: Trigger allows you to define downstream pipeline trigger.

### Harness

[Harness](https://harness.io/) is a Continuous Delivery as a Service platform 
which enables confidence building orchestration and release strategies across a 
multitude of platforms. 

Some of the core Harness terms are listed below. [[15]]

- **Manager**: Where your deployment configurations are stored and pipelines are managed.
Either available as a SaaS or on-prem. 
- **Delegate**: Worker node that is installed in your environment which performs Continuous
Delivery tasks by connecting to your infrastructure. 
- **Application**: How a deployment project is organized. 
- **Service**: Represent your microservices and applications. 
- **Environment**: Represent your deployment infrastructure e.g Dev, QA, Prod. 
- **Workflow**: Model how your application is deployed, verified, and rolled back in steps. 
- **Pipeline**: Model your entire release process in stages. 
- **Infrastructure Provisioner**: Infrastructure as code orchestration. 

### Jenkins

[Jenkins](https://jenkins.io/) is an open source automation server which
enables developers around the world to reliably build, test, and deploy their
software.

Some of the core Jenkins terms are listed below. [[4]]

- **Job**: A user-configured description of work which Jenkins should
perform, such as building a piece of software, etc.
- **Project**: A deprecated term, synonymous with Job.
- **Stage**: Stage is part of Pipeline, and used for defining a conceptually
distinct subset of the entire Pipeline
- **Pipeline**: A user-defined model of a continuous delivery pipeline (see [Jenkins Pipeline](https://jenkins.io/doc/book/pipeline/)).
- **Agent**: A machine or a container which is connected to the Jenkins master and capable of executing Pipelines or Jobs.
Both the Master and Agents are considered to be Nodes.
- **Node**: A machine or a container which is part of the Jenkins environment and capable of executing Pipelines or Jobs.
Both the Master and Agents are considered to be Nodes.
- **Trigger**: A criteria for triggering a new Pipeline run or a Job.

### Jenkins X

[Jenkins X](https://jenkins-x.io/) provides pipeline automation, built-in
GitOps, and preview environments to help teams collaborate and accelerate
their software delivery at any scale.

Some of the core Jenkins X terms are listed below. [[5]]

- **Step**: Basic building block to execute one or more commands.
- **Stage**: Collection of steps and the required configuration.
- **Pipeline**: Collection of one or more stages to run.
- **Agent**: Container image or Jenkins agent to schedule pipelines on.
- **Trigger**: A pipeline trigger defines when to automatically run a pipeline.

### Keptn

[Keptn](https://keptn.sh/) is an event-based control plane for continuous delivery and automated operations for cloud-native applications.

Some of the core Keptn terms are listed below. [[6]]

- **Shipyard:** A shipyard is the declarative means to divide an environment into stages and to specify workflows for each stage.
- **Workflow**: A workflow declares a set of tasks for implementing a delivery or operations process. A workflow is triggered by an external event, i.e., by a *domain event*. Examples for domain events would be the availablity of a new artifact that should be deployed (i.e., a `new-artifact` event) or the occurence of a problem (i.e., a `problem` event).
- **Task**: A task is the smallest executable unit in a workflow. A task is triggered by an event.
- **Event**: An event triggers a task and contains relevant data for the respective task.
- **Keptn-service:** A Keptn-service is the unit executing a task. It can be responsible for executing one or many tasks and is triggered by an event of a task.

### Screwdriver

[Screwdriver](https://screwdriver.cd) is an open source build platform designed
for Continuous Delivery.

Some of the core Screwdriver terms are listed below. [[7]]

- **Step**: List of commands to execute.
- **Job**: Collection of the steps to run.
- **Workflow**: Collection and order of jobs to run.
- **Pipeline**: Used interchangeably with workflow. (*citation needed*)
- **Trigger**: A pipeline trigger defines when to automatically run a pipeline
or job. (*citation needed*)

### Spinnaker

[Spinnaker](https://www.spinnaker.io/) is an open source, multi-cloud continuous
delivery platform for releasing software changes with high velocity and
confidence.

Some of the core Spinnaker terms are listed below. [[8]]

- **Task**: An atomic function to perform.
- **Stage**: A collection of sequential Tasks and composed Stages that describe
a higher-level action the Pipeline will perform either linearly or in parallel.
- **Pipeline**: The pipeline is the key deployment management construct in
Spinnaker. It consists of a sequence of actions, known as stages.
- **Pipeline Template**: A parameterized pipeline, minus the pipeline
configuration found on a pipeline instance. This template helps developers
create pipelines that follow a pattern that you establish.
- **Pipeline configuration**: The same as the configuration for a pipeline
not created from a template, plus variable bindings and a reference to the
template.
- **Cluster**: Logical groupings of Server Groups in Spinnaker.
- **Provider**: A Cloud Provider is an interface to a set of virtual resources
that Spinnaker has control over.
- **Trigger**: A pipeline trigger defines when to automatically run a pipeline.

### Tekton

[The Tekton Pipelines](https://github.com/tektoncd/pipeline) project provides
k8s-style resources for declaring CI/CD-style pipelines.

Some of the core Tekton terms are listed below. [[9]]

- **Step**: a specific function to perform.
- **Task**: is a collection of sequential steps you would want to run as part
of your continuous integration flow. A task will run inside a pod on your cluster.
- **ClusterTask**: Similar to Task, but with a cluster scope.
- **Pipeline**: stateless, reusable, parameterized collection of tasks. Tasks are
linked together in a Pipeline, which describes the end-to-end deployment for an application.
- **PipelineRun**: an instantiation of a Pipeline definition, filling in the 
Pipeline's parameters with concrete values
- **Pipeline Resource**: objects that will be input to or output from tasks
- **Trigger**: Triggers is a Kubernetes Custom Resource Defintion (CRD) controller 
that allows you to extract information from event payloads (a "trigger") to create Kubernetes resources.

### Zuul

[Zuul](https://zuul-ci.org/) is a program that drives continuous integration,
delivery, and deployment systems with a focus on project gating and
interrelated projects.

Some of the core Zuul terms are listed below. [[10]]

- **Job**: A job is a unit of work performed by Zuul on an item enqueued into
a pipeline.
- **Pipeline**: A pipeline describes a workflow operation in Zuul.
It associates jobs for a given project with triggering and reporting events.
to one or more projects.
- **Trigger**: Descriptions of events which should cause something to be
enqueued into a pipeline.
- **Node**: Virtual or static machines where the jobs are scheduled on.
- **Executor**: Executors are responsible for running jobs.

## Terminology Used by SCM Tools and Technologies

This section contains list of some key terms of various SCM tools and
technologies.

### Gerrit

[Gerrit](https://www.gerritcodereview.com/) is a free, web-based team code
collaboration tool.

Some of the core Gerrit terms are listed below. [[11]]

- **Change**: The unit of review. Results in a single commit when merged
to the Git repository. Change numbers (identifiers) are unique and never
change.
- **Patch Set**: A revision of a Change. Each time a Change is modified,
it will receive a new Patch Set. Patch Set numbering starts from 1.
Technically, a Patch Set is a unique Git commit.
- **Review**: Process that enables peer-review to improve the quality of
code.
- **Approval Category**: Name for a scope that is checked during review
process. Could be given by reviewers or CI/CD processes.
- **Submit**: An action that allows Gerrit to merge a Change to the Git
repository.

### GitHub

[GitHub](https://www.github.com) is a hosted software development version
control system using Git.

Some of the core GitHub terms are listed below. [[12]]

- **Pull Request**: Proposed changes to a repository submitted by a user
and accepted or rejected by a repository's collaborators.
- **Review**: Process that enables peer-review to improve the quality of
code.
- **Status Check**: Status checks are external processes, such as continuous
integration builds, which run for each commit you make in a repository.
- **Check**: A check is a type of status check on GitHub.
- **Merge**: Acceptance of a PR by the maintainers.

### GitLab

[GitLab](https://www.gitlab.com) is a web-based DevOps lifecycle tool that
provides a Git-repository manager providing wiki, issue-tracking and CI/CD
pipeline features.

Some of the core GitLab terms are listed below. [[13]]

- **Merge Request**: MR is the basis of GitLab as a code collaboration and
version control platform. It is as simple as the name implies: a request to
merge one branch into another.
- **Review**: Process that enables peer-review to improve the quality of
code.
- **Merge Check**: Checks to ensure MR can be merged without issues.
- **Merge**: Acceptance of a MR by the maintainers.

## Mapping of Terms

The Tools and Technologies listed in this document use more or less same
terminology for naming things with few differences, workflow vs pipeline or
runner vs node except the smaller units of work.

Fields marked as *N/A* in the tables below means that the author of this
document failed to identify corresponding term in the documentation of those
tools and does not mean those units of work are not supported by the tools.
Fields containing a question mark is the author's guess and might be incorrect.

### CI/CD Tools and Technologies

The table below is an attempt to create a mapping of different terms used
by CI/CD Tools and Technologies and could contain errors. The main term used
while creating the table is **pipeline** since almost all the tools listed in
this document use the word pipeline to describe pretty similar things. Smaller
units of terms then mapped based on how they are described in relation to
pipeline in corresponding documentation.

| Project            |          |          |          |          |         |              |
|--------------------|----------|----------|----------|----------|---------|--------------|
| **ArgoCD**         | Sync Wave         | Sync Phase  | Sync      |N/A      | Event         |  Application Controller            |
| **CircleCI**       | N/A      | Step     | Job      | Workflow | Trigger | Executor     |                    |          |          |          |          |         |              |
| **Eiffel**         | Activity | Activity | Activity | Activity | Event   | Environment  |
| **GitHub Actions** | Action   | Step     | Job      | Workflow | Event   | Runner       |
| **GitLab CI/CD**   | N/A      | Job      | Stage    | Pipeline | Trigger | Runner       |
| **Harness**        | N/A      | Step     | Pipeline | Workflow | Trigger | Delegate     |
| **Jenkins**        | N/A      | Job      | Stage    | Pipeline | Trigger | Agent/Node   |
| **Jenkins X**      | N/A      | Step     | Stage    | Pipeline | Trigger | Agent        |
| **Keptn**          | N/A      | N/A      | Task     | Workflow | Event   | Keptn-service|
| **Screwdriver**    | N/A      | Step     | Job      | Pipeline | Trigger | N/A          |
| **Spinnaker**      | N/A      | Task     | Stage    | Pipeline | Trigger | Cluster      |
| **Tekton**         | N/A      | Step     | Task     | Pipeline | Trigger | Resource (?) |
| **Zuul**           | N/A      | N/A      | Job      | Pipeline | Trigger | Node (?)     |

### SCM Tools and Technologies

The table below is an attempt to create a mapping of different terms used
by SCM Tools and Technologies.

| Project    |               |               |          |               |        |
|------------|---------------|---------------|----------|---------------|--------|
| **Eiffel** | (Change)      | Source Change | Activity | N/A           | Submit |
| **Gerrit** | Change        | Patch Set     | Review   | Change State? | Submit |
| **GitHub** | Pull Request  | (PR commit)   | Review   | Check?        | Merge  |
| **GitLab** | Merge Request | (MR commit)   | Review   | Merge Check?  | Merge  |

## Shared Vocabulary

TBD

[1]: https://circleci.com/docs/2.0/glossary/
[2]: https://help.github.com/en/actions/automating-your-workflow-with-github-actions/core-concepts-for-github-actions
[3]: https://about.gitlab.com/blog/2019/07/12/guide-to-ci-cd-pipelines/
[4]: https://jenkins.io/doc/book/glossary/
[5]: https://jenkins-x.io/docs/concepts/
[6]: https://keptn.sh/docs/0.6.0/concepts/glossary/
[7]: https://docs.screwdriver.cd/user-guide/quickstart
[8]: https://www.spinnaker.io/concepts/
[9]: https://github.com/tektoncd/pipeline/blob/master/docs/README.md
[10]: https://zuul-ci.org/docs/zuul/discussion/concepts.html
[11]: https://wiki.qt.io/Gerrit_Introduction#Terminology
[12]: https://help.github.com/en/github/getting-started-with-github/github-glossary
[13]: https://docs.gitlab.com/ee/user/project/merge_requests/
[14]: https://github.com/eiffel-community/eiffel/tree/master/eiffel-vocabulary
[15]: https://docs.harness.io/article/4o7oqwih6h-harness-key-concepts
[16]: https://argoproj.github.io/argo-cd/core_concepts/
[17]: https://argoproj.github.io/argo-cd/user-guide/projects/
[18]: https://argoproj.github.io/argo-cd/user-guide/sync-waves/
[19]: https://argoproj.github.io/argo-cd/operator-manual/architecture/