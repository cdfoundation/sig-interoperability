# Events in CICD Workstream Meeting Notes

The first meeting in this workstream is scheduled for June 8th, at 6.30pm CET

The forming of this workstream was suggested on last weeks SIG Interoperability meeting: https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings.md#may-28-2020

## Meeting June 8th

Participants:
* Ravi Lachhman, Harness
* Ramin Akhbari, eBay
* Andreas Grimmer, Dynatrace
* Emil Bäckmark, Ericsson
* Emelie Pettersson, Ericsson

Recording: https://ebay.zoom.us/rec/share/9O9TNa3C2HtJAdbs9HjBc4wwOJTbT6a81XJK86ZbmhlxbyK0_xpQnMmRfY5QWq-O


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


