# Events in CICD Workstream Meeting Notes

This workstream meet every second Monday at 16.30 UTC  (See your timezone [here](https://time.is/1630_in_UTC)). Register in advance for this meeting and get an invite to your calendar:
https://zoom.us/meeting/register/tJMrcemvrzksGtSgbE3-44y5nBvCkKI6X2MT

The forming of this workstream was suggested on a [recent SIG Interoperability meeting]( https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings.md#may-28-2020) and its first meeting was held on June 8th.

Meeting notes for the workstream are managed on HackMD [here](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w), and published to GitHub [here](https://github.com/cdfoundation/sig-interoperability/blob/master/workstreams/events_in_cicd/meetings.md).

## Meeting July 6th

### Topics

#### What is an event?
* Third iteration of this topic :)
* What does cloudevents mean with events?

#### Common vocabulary
* What's the next step with the 'Rosetta Stone'? Frameworks/tools missing there?

#### Existing event handling frameworks
The million dollar question is what to publish!

* Tekton Triggers
* [Keptn](https://keptn.sh/)
* [Eiffel](https://eiffel-community.github.io/)
* [Cloud Events](https://cloudevents.io/)
* [Argo Events](https://github.com/argoproj/argo-events)

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


