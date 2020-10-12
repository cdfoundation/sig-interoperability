# Events in CICD Workstream Meeting Notes

[![hackmd-github-sync-badge](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w/badge)](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w)


This workstream meet every second Monday at 16.30 UTC  (See your timezone [here](https://time.is/1630_in_UTC)). Register in advance for this meeting and get an invite to your calendar:
https://zoom.us/meeting/register/tJMrcemvrzksGtSgbE3-44y5nBvCkKI6X2MT

The forming of this workstream was suggested on a [recent SIG Interoperability meeting]( https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings.md#may-28-2020) and its first meeting was held on June 8th.

Meeting notes for the workstream are managed on HackMD [here](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w), and published to GitHub [here](https://github.com/cdfoundation/sig-interoperability/blob/master/workstreams/events_in_cicd/meetings.md).

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


