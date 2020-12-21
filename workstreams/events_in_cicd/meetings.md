# Events in CICD Workstream Meeting Notes

[![hackmd-github-sync-badge](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w/badge)](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w)


This workstream meet every second Monday at 16.00 UTC  (See your timezone [here](https://time.is/1600_in_UTC)). The meeting can be accessed through this zoom link: https://zoom.us/j/97660712600?pwd=Z3BqYTE5YzNsbEhmck16cjdZNEFIUT09

The forming of this workstream was suggested on a [recent SIG Interoperability meeting]( https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings.md#may-28-2020) and its first meeting was held on June 8th.

Meeting notes for the workstream are managed on HackMD [here](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w), and published to GitHub [here](https://github.com/cdfoundation/sig-interoperability/blob/master/workstreams/events_in_cicd/meetings.md).


## Meeting December 21th
Meeeting time in your timezone [here](https://time.is/1600_7_December_2020_in_UTC). You're welcome to join!

Participants:
- Emil Bäckmark, Ericson
- Andreas Grimmer, Dynatrace
- Ravi Lachhman, Harness
- Andrea Frittoli, IBM
- Mauricio Salatino, Camunda / LearnK8s

### Agenda and Notes

#### Charter
- On December 7th, we decided on working on a charter for our workstream. You can find the working document [here](https://docs.google.com/document/d/1cuaOHmrvK20WxHxHZZuLif3CW3q1ICZ_RglJRp_IAQ0/edit?usp=sharing)
- Main focus areas for the Events SIG
  - Defining a protocol, and documenting it
  - Providing how to apply the protocol in different use cases, such as monitoring, triggering activities, audits, etc
  - Providing a reference implementation of services/libraries showcasing the protocol
- We should all review and contribute to the charter before or on the next meeting

#### CD-Flow
Mauricio will provide a presentation on this work in a later meeting
- https://github.com/salaboy/cd-flow/ 

#### FOSDEM CI/CD Devroom

It could be nice to present the work of this group at [FOSDEM 2021](https://fosdem.org/2021/schedule/track/continuous_integration_and_continuous_deployment/).
The CFP closes on Dec 27, the conference takes place (virtually) on 6, 7 Feb 2021.

#### cdCon 2021
We should contribute to it
- cdCon will be in June
- CFP (not open yet)
- 'Event driven CI/CD' could be a valid topic
- https://events.linuxfoundation.org/cdcon/

#### Other conferences
Online DevOps online summit, on Slack. Tracy has been asked to set up a CI/CD channel for it.
- https://devopsonlinesummit.com/

#### Contribute to Metadata workstream
Metadata workstream is about to get started and we should provide any input we have that relates to metadata to it: [Standardized Metadata](https://hackmd.io/BYbkuR8uSlKt_w7Y4KE1OQ)
- We never discussed this agenda point at this meeting

#### Next Meeting
4th of January is skipped so first meeting after new year will be 18th of January? Or do we want a meeting before the TOC meeting where the workstream becoming a SIG will be lifted? When is the next SIG Interop meeting?
AP Emil: Ask Tracey/Fatih to cancel the meeting January 4th

## Meeting December 7th
Meeeting time in your timezone [here](https://time.is/1600_7_December_2020_in_UTC). You're welcome to join!

Participants:
* Ravi Lachhman, Harness
* Andreas Grimmer, Dynatrace
* Emil Bäckmark, Ericsson
* Steve Taylor, DeployHub
* Mattias Linnér, Ericsson
* Tracy Ragan, DeployHub
* Andrea Frittoli, IBM

### Agenda and Notes

#### Use Cases from DeployHub on this workstream
- Interested in seeing some of the CDF projects move into an event driven pipeline
- Ortelius keeps track of deliveries that are to be deployed and their relationships
    - Generate workflows on the fly
    - Events should be propagated saying for example 'I have completed this step'

#### Events in CICD Workstream to become SIG?
Let's continue the discussion on this idea brought up on last meeting.
- What about the relation to SIG Interoperability? To workstream Metadata? Others?
- Having a SIG means a bit more formality and also provides more visibility of the group.
- To Do: Level of effort and commitments for Working Group vs SIG. 
    - Having a SIG might attract more volunteers
- A charter would be needed for a SIG. We would benefit from creating a charter, given a clear scope and direction
    - We should work on the charter regardless of if we become a SIG or not
    - AP Andreas: Set up a Google docs where we could initiate the charter work
- There is a risk that this group could be slowed down due to the extra work needed
- What about the metadata workstream? Should it be part of this new SIG or SIG Interop?
- Sig Interop Charter: https://github.com/cdfoundation/sig-interoperability/blob/master/docs/roadmap.md#charter
- We should join the TOC in January to discuss this
    - Tracy will ask for us to get a point on the agenda for January 19th. No preparations needed from our end.
- Should SIG Interop be renamed to SIG events or should there be a separate SIG for it?
- Sig Repo: https://github.com/cdfoundation/sig-interoperability

#### cdCon 2021
We should contribute to it
- cdCon will be in June
- CFP is not there yet
- 'Event driven CI/CD' could be a valid topic

#### Other conferences
- Online DevOps online summit, on Slack. Tracy has been asked to set up a CI/CD channel for it.
    - https://devopsonlinesummit.com/

#### Contribute to Metadata workstream
Metadata workstream is about to get started and we should provide any input we have that relates to metadata to it: [Standardized Metadata](https://hackmd.io/BYbkuR8uSlKt_w7Y4KE1OQ)
- We never discussed this agenda point at this meeting

#### Events Vocabulary
Let's progress the vocabulary discussions
- We never discussed this agenda point at this meeting

#### Next Meeting
Ok to meet December 21st, or should we postpone it till after xmas? What about Monday 4th of January in Epiphany week?
- Decided to meet December 21st
- 4th of January is skipped so first meeting after new year will be 18th of January

## Meeting November 23rd
Meeeting time in your timezone [here](https://time.is/1600_23_November_2020_in_UTC). You're welcome to join!

Participants:
* Ravi Lachhman, Harness
* Emil Bäckmark, Ericsson
* Mattias Linnér, Ericsson
* Cameron Motevasselani, Armory
* Andrea Frittoli, IBM
* Andreas Grimmer, Dynatrace
* Tracy Ragan, DeployHub

### Meeting Time
It was decided through a Slack discussion to move our meetings to 16.00 UTC starting from this meeting.

### Agenda

#### The life of this worksteam
- TR: Should this workstream be lifted to become it's own SIG? It would benefit the group and also CDF
- We should collect input from the SIG Interop about this idea on Thursday.
- The idea of lifting this to its own SIG should also be lifted to Dan Lorenc, to be discussed on the TOC level
- Suggested scope
    - What would an event driven CICD 'practice' look like?
    - Focusing on the event protocol or a higher level? Also including events infrastructure?
    - Focusing on a common events listener? Or instead of a provided events listener, it could be a layer on top of an existing cloudevents library meant to listen to and parse events in certain libraries
- We should get in people from Puppet as well, CircleCI, Argo, Codefresh, JFrog, Gitlab. And of course the existing: Harness, Keptn, Ortelius, Spinnaker, Weaveworks (for Flagger). And end-users like Ramin (eBay)
- Focus on tools for orchestration/workflows or also release/delivery/deployment tools?
- TR: Reasons for events in Ortelius
    - Regardless of platform used, the workflows should be able to state their progress and risk levels in a generic way. To enable 'smart CD pipelines'

#### Note:
- Member webinar around events next week (see CDF Calendar): 'CDF Ambassador Webinar: A Guide to Event-driven SRE-inspired DevOps', Wednesday December 2nd
- https://docs.google.com/document/d/11EZfvB2FFI837nMmArnyv-wizsIJvc-4_xdgfoUXF4o/edit?ts=5fb68361#heading=h.mspta0kuuv9j

#### Is the discussion frequency good as it is or should we increase it, through using the Slack channel or comments in the HackMD document?
- Discussion to be continued on this topic when/if the workstream is lifted to it's own SIG

#### Metadata group
- What about [the Standardized Metadata discussion](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings.md#agenda-and-notes-1) that was brought up on last SIG meeting? How should it relate to our work in this workstream?
- If events in CICD will become a SIG then maybe the metadata group should be part of it 

### Community Specification
- [Community Specification](https://github.com/CommunitySpecification/1.0), would it be interesting for us to use?
    - It's about getting a head start in defining a new specification. Taking care of legal aspects etc.
    - It could be cloned or linked to from a new specification that we create for events
    - What about Cloudevents? Do they use this? Why? Why not?
    - It might already be covered within CDF, and therefore we might not need it. Should be asked to Tracy Miranda


## Meeting November 9th
Meeeting time in your timezone [here](https://time.is/1630_9_November_2020_in_UTC). You're welcome to join!

Participants:
* Emil Bäckmark, Ericsson
* Mattias Linnér, Ericsson
* Andreas Grimmer, Dynatrace

### Meeting time
As it seems to be hard for some members to join at this time, we propose that it is rescheduled to 15.00 UTC instead (same time as SIG meeting on Thursdays). This is posted on Slack in a comment as well.

### Suggested Agenda
- Is the discussion frequency good as it is or should we increase it, through using the Slack channel or comments in the HackMD document?
- What about [the Standardized Metadata discussion](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings.md#agenda-and-notes-1) that was brought up on last SIG meeting? How should it relate to our work in this workstream? 
- [Community Specification](https://github.com/CommunitySpecification/1.0), would it be interesting for us to use?

## Meeting October 26th
Meeeting time in your timezone [here](https://time.is/1630_26_October_2020_in_UTC). You're welcome to join!

Participants:
* Emil Bäckmark, Ericsson
* Mattias Linnér, Ericsson
* Andrea Frittoli (IBM)
* \<add yourself\>

### Agenda

#### Meeting time
- Should we stick to 16.30 UTC or should we move the meeting in accordance with daylight savings time in some way?
- AP Emil: Bring this question to Slack

#### Events Vocabulary
https://hackmd.io/B-Z7mLh_Qc6frm51f3GIYA

- We restructured the discussion section a bit
- How should we document our discussions? Group on different topics? Timestamp? 


## Meeting October 12th
Meeeting time in your timezone [here](https://time.is/1630_12_October_2020_in_UTC). You're welcome to join!

Participants:
* Emil Bäckmark (Ericsson)
* Ravi Lachhman (Harness)
* Andrea Frittoli (IBM)

### Topics

#### Meeting setup and recordings
The meeting can now be joined without the Zoom client 

#### Events Vocabulary
https://hackmd.io/B-Z7mLh_Qc6frm51f3GIYA


## Meeting September 28th
Meeeting time in your timezone [here](https://time.is/1630_28_September_2020_in_UTC). You're welcome to join!

Participants:
* Andreas Grimmer (Dynatrace)
* Emil Bäckmark (Ericsson)
* Mattias Linnér (Ericsson)

### Suggested Topics

#### Meeting setup and recordings
AP Emil: Check with Jackie (or Tracey) on if this meeting can be held as a zoom browser meeting or just with the Zoom client. What about the recording, where is it stored? Should it be on Youtube?

#### Finalize contribution to SIG Whitepaper
https://docs.google.com/document/d/10m0LVTSAqltN2xNATwKS6dU8cMx08Co9-dnvvsIXD8M/edit
The contribution was reviewed during the meeting and moved to the [actual whitepaper](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit#).

#### Events Vocabulary
https://hackmd.io/B-Z7mLh_Qc6frm51f3GIYA

## Meeting September 14th
Meeeting time in your timezone [here](https://time.is/1630_14_September_2020_in_UTC). You're welcome to join!

Participants:
* Emil Bäckmark (Ericsson)
* Mattias Linnér (Ericsson)
* Andreas Grimmer (Dynatrace)
* Andrea Frittoli (IBM)

### Topics

#### SIG Interop Whitepaper
Our contribution: https://docs.google.com/document/d/10m0LVTSAqltN2xNATwKS6dU8cMx08Co9-dnvvsIXD8M/edit

Tekton project with event pipelines: https://github.com/tektoncd/plumbing

#### Events Vocabulary
https://hackmd.io/B-Z7mLh_Qc6frm51f3GIYA

## Meeting August 31st
Meeeting time in your timezone [here](https://time.is/1630_31_August_2020_in_UTC). You're welcome to join!

Participants:
* Emil Bäckmark (Ericsson)
* Ravi Lachhman (Harness)
* Mattias Linnér (Ericsson)
* Andreas Grimmer (Dynatrace)
* Max Körbächer (Storm Reply)

### Potential Topics 

#### Kubecon Europe

https://events.linuxfoundation.org/kubecon-cloudnativecon-europe/

Anyone who joined? Anything to share w.r.t. events in CI/CD?

- Weaveworks presented a new version of CD GitOPS

#### Common Vocabulary

- Recap of last meeting discussion

- Activity Started
  - Live Logs
- Activity Finished
  - Status SUCCEEDED/...
  - Result PASSED/FAILED
  - Persistant Logs
- Activity Canceled
- Activity Triggered

- Status Changed (informs e.g. about Y test cases executed or X canary releases performed)
  - Context: Refers to the system on which the state is changed

- Collect input from Eiffel, Keptn, Tekton. And more?

- AP on all: Read up on existing frameworks (linked in earlier minutes) and propose high level event terminology

- AP Emil: Prepare Hackmd document for the proposal and share with the group


#### SIG Interop Whitepaper
???
https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit#


## Meeting August 17th
Meeeting time in your timezone [here](https://time.is/1630_17_August_2020_in_UTC). You're welcome to join!

Participants:
* Emil Bäckmark (Ericsson)
* Ravi Lachhman (Harness)

### Common Vocabulary
Time to push (parts of?) this?

One way to start is to define some use cases to report events using. Proposal: go for the Eiffel terminology for 'Activities'.
https://github.com/eiffel-community/eiffel/tree/master/eiffel-vocabulary

#### Basic For All to Understand #####
* Start
    * URI (link to ongoing execution)
    * LiveLogs (links to active logs)
* Finish
    * Outcome
        * Fail
        * Success
    * PersistantLogs (links to finished logs)

#### Intermediate for CI/CD Knowledge #####
* Trigger
    * Name
* Cancel
* Alerting/Monitoring/Still Processing 
    *  URI (link to ongoing execution)

#### Links and/or contexts
* How to connect events to each other and to the source change or other item that triggered their actions? (SIG Feedback please!) AP Emil: Present the Eiffel link model in  a coming meeting.

We should create:
* Schema
* Specification 
* JSON/API Docs for visualization (e.g Swagger) e.g https://www.gremlin.com/docs/api-reference/overview/

### SIG Interop Whitepaper
What should we contribute to it?
* White Paper for SIG: https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit#


## Meeting July 6th
Meeeting time in your timezone [here](https://time.is/1630_22_June_2020_in_UTC). You're welcome to join!

Participants:
* Andreas Grimmer (Dynatrace)
* Ravi Lachhman (Harness)
* Emil Bäckmark (Ericsson)
* Ramin Akhbari (eBay)
* Marky Jackson (OpsMX)

### Topics

#### What is an event? vs. Message, Notification, ...
* Tried these definitions:
  * An event is something of interest that has happened in the past
  * A notification is a container describing such an event, to be sent over some messaging line
* What does cloudevents mean with events?
  * Cloudevents define 'occurrence' and 'event': [Cloudevents terminology](https://github.com/cloudevents/spec/blob/v1.0/spec.md#terminology)
* **We decided to stick with the [Cloudevents definitions]((https://github.com/cloudevents/spec/blob/v1.0/spec.md#terminology)) for now**

#### Common vocabulary
* What's the next step with the 'Rosetta Stone'? Frameworks/tools missing there?
* Event: Something of interest that has occured in the past in a particular domain. 
* Eiffel Vocab (https://github.com/eiffel-community/eiffel/tree/master/eiffel-vocabulary)

#### What is working well in the Industry?
* Keptn is event driven.Follows Cloud Events spec. (https://github.com/cloudevents/spec/blob/v1.0/spec.md)

#### Existing event handling frameworks
What event frameworks do we know of?

##### Pure event consumers
* [Tekton Triggers](https://medium.com/@dlorenc/tekton-triggers-3aba132c6344)
* [Argo Events](https://github.com/argoproj/argo-events)
* Various [Eiffel consumers](https://eiffel-community.github.io/)
* Others?

##### Pure event producers
* Various [Eiffel producers](https://eiffel-community.github.io/)
* Others?

##### Both producers and consumers 
* [Keptn](https://keptn.sh/) ?
* Tekton - Consumer [Tekton Triggers](https://medium.com/@dlorenc/tekton-triggers-3aba132c6344), Producer [Tekton event sending](https://github.com/tektoncd/pipeline/releases/tag/v0.14.0)

##### Event protocol standards (for consumers and producers)
* [Eiffel](https://eiffel-community.github.io/)
* [CloudEvents](https://cloudevents.io/)

### Brainstorming event formats
* Event 101, "Hello SIG"


## Meeting June 22nd
Meeeting time in your timezone [here](https://time.is/1630_22_June_2020_in_UTC). You're welcome to join!

Participants:
* Ravi Lachhman, Harness
* Andreas Grimmer, Dynatrace
* Emil Bäckmark, Ericsson
* Ramin Akhbari, eBay
* Andrea Frittoli, IBM

### Topics
* Tekton Events: (Need to join the SIG/Get Access) https://docs.google.com/document/d/1ehhGngn2ulnjYX0HUxSyhQGAvcbabSa27UZs3RvZWwU/edit#heading=h.fekiyq267j9v
* Google Group -> https://groups.google.com/forum/#!forum/tekton-dev
* Tekton Triggers (Easy Reading) https://medium.com/@dlorenc/tekton-triggers-3aba132c6344
* Readme doc: https://hackmd.io/AnVkdMb3QEeVQXKfIj4tNQ
 
#### My First Event aka Hello/MVP Event
What would be the very first event? 

* Start/Stop
* Error
* Pause
* Regression
* etc

Tekton Trigger Start/Stop: https://github.com/tektoncd/pipeline/issues/742

#### What is an event?
* We re-iterated this discussion from last meeting.
* Is an even only what occurs in the (CD) system? Or is it also the entity that is sent out from the system at that point? Or is that a 'Notification' about the event that occured?
* To be continued in next meeting

## Meeting June 8th

Participants:
* Ravi Lachhman, Harness
* Ramin Akhbari, eBay
* Andreas Grimmer, Dynatrace
* Emil Bäckmark, Ericsson
* Emelie Pettersson, Ericsson

Recording: https://youtu.be/l7YrA7kBw7I

The intention with this initial meeting is to get a common understanding of what areas to cover in this workstream and to identify the way forward for the workstream.

Zoom Bridge: https://ebay.zoom.us/j/95990976381
Timezone help: https://time.is/compare/1830_8_June_2020_in_CET/EST/PST

# Why we are here?
* Unique benefits of Event-driven CD pipelines
* Automation of CD processes

# Discussion
* Pipeline to Pipeline Communication 
* Context sent to decisions/Pipelines
* What is an event? - Cloud Events Project -> https://cloudevents.io/
* Message/Envelope: Long lived and routable. 
* Event: Immediate, consumable. An indication. 
* Structure of an Event (definition).
* Technology agnostic to what to be deploying to. 
* Harmonization of verbiage/vocabulary. -> https://github.com/cdfoundation/sig-interoperability/blob/master/docs/vocabulary.md
* When to Event? Trigger, Audit, Monitoring, Management
* Graphing of the entire process e.g through events. What truly occurs? 
* Metrics about Events; e.g how many people have subscribed? Alerting around Events. 

# Workstream name
We concluded to rename the workstream to 'events in CI/CD' to not narrow the scope of the work to just triggering or driving pipelines

# Next Steps
* Bi-Weekly Meetings at same time.
* Read up on the CDF SIG Interop vocabulary document - https://github.com/cdfoundation/sig-interoperability/blob/master/docs/vocabulary.md
* Read up on events proposal for Tekton - Ramin to provide link
* RA: Here's the link to Andrea Frittoli’s Actions and Notifications proposal:
https://docs.google.com/document/d/1ehhGngn2ulnjYX0HUxSyhQGAvcbabSa27UZs3RvZWwU


