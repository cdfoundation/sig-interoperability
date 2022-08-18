###### tags: `SIG Interoperability`

# CDF Interoperability SIG Meetings

[![HacmKD documents](https://hackmd.io/badge.svg)](https://hackmd.io/HuufSDMaTPyb3qxkyBKg3A?edit)

## Quick links

* [Logistics](#Logistics)
* [Meeting Recordings](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG)
* [Agenda and Notes](#Agenda-and-Notes)
    * [2022-08-18 Meeting](#August-18-2022)
    * [2022-08-04 Meeting](#August-4-2022)
    * [2022-07-21 Meeting](#July-21-2022)
    * [2022-07-07 Meeting](#July-7-2022)
    * [2022-06-16 Meeting](#June-16-2022)
    * [2022-06-02 Meeting](#June-2-2022)
    * 2022-05-19 Meeting (Cancelled)
    * 2022-05-05 Meeting (Cancelled)
    * [2022-04-21 Meeting](#April-21-2022)
    * [2022-04-07 Meeting](#April-7-2022)
    * [2022-03-17 Meeting](#March-17-2022)
    * [2022-03-03 Meeting](#March-3-2022)
    * [2022-02-17 Meeting](#February-17-2022)
    * [2022-02-03 Meeting](#February-3-2022)
    * [2022-01-20 Meeting](#January-20-2022)

## Logistics

* **Meeting notes on HackMD.io**: https://hackmd.io/@cdfoundation/ry3TTB5DL
* **When**: First and third Thursdays at [3pm UTC](https://time.is/3pm_in_UTC) during summer time and at [4pm UTC](https://time.is/4pm_in_UTC) during winter time).
* **Zoom Bridge**: https://zoom.us/j/827082528?pwd=RlN5OUZtVVBuZGZRY0NBRnZyZ0NJQT09
* **Zoom International dial-in numbers**: https://zoom.us/zoomconference
* **Meeting Recordings**: [CDF Youtube Channel SIG Interoperability Playlist](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG)
* **CDF Public Calendar**: [here](https://calendar.google.com/calendar/embed?src=linuxfoundation.org_mhf0kmgedn67ihni8r129avp24%40group.calendar.google.com&ctz=America%2FLos_Angeles)
* **Past Presentations in CDF Presentations Repository**: https://github.com/cdfoundation/presentations/tree/master/sig-interoperability
* **Presentation Schedule**: https://docs.google.com/document/d/1Owg_I52WEXzqF8g_lX6OTdwbHkH4Z2-7TBA7eCSVMqY/edit
* **2021 Meeting Minutes**: https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings_2021.md
* **2020 Meeting Minutes**: https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings_2020.md

## Agenda and Notes

Meeting agenda and notes are kept on [HackMD.io](https://hackmd.io/@cdfoundation/ry3TTB5DL) where everyone can add new topics to the agenda for upcoming meetings or take notes during the meetings. Please click edit button to edit the document.

If you are looking for 2021 minutes of meetings, please take a look at [Meetings 2021 document](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings_2021.md) in SIG Interoperability repository on GitHub.

### August 18, 2022

#### Participants
* \<AddMe\>

#### Agenda & Notes
* Open Action Items (outstanding from previous meetings)
    * Justin: Intent based pipelines article
    * Melissa: Determine WHERE in the best practices site to add vocabulary documentation (https://bestpractices.cd.foundation/); Review Terry's suggestions from last meeting
    * Fatih & Ann Marie: address vocabulary split and conflicts in outstanding PRs
    * CDEvents and Pipeline terminology alignment
* Other announcements
    * JReleaser will be presenting Sep 1
    * Our github default branch has been renamed from master to main - thank you Kara!
* \<Add\>

### August 4, 2022

#### Participants
* Melissa McKay, JFrog
* Kara de la Marck, CDF
* Tim Miller, Kusari

#### Agenda & Notes
* Reference Architecture discussions will be continued in the Best Practices SIG (possibly a new working group)
* New projects to present to the SIG
    * go-scm - [ACTION] agree on a scheduled time for presentation
    * JReleaser - schedule presentation Sep 1
* FRSCA Project - https://github.com/buildsec/frsca
    * [ACTION] - schedule a presentation
* [CDF Landscape](https://github.com/cdfoundation/cdf-landscape)
    * We welcome PRs to add projects -- JReleaser now added 
    * If you feel a category is missing, please raise an issue


### July 21, 2022

#### Participants
* Justin Abrahms, eBay
* Kara de la Marck, CDF
* Fatih Degirmenci, CDF
* Terry Cox

#### Agenda & Notes
* Reference Architecture chat
    * [deck around what a reference architecture is](https://docs.google.com/presentation/d/1SSSHPLSXEUgg0vu644zrZPvCW9sUYSBwzSCDO_fZtF8/edit#slide=id.g13b9833d9a3_0_28)
    * current docs/projects are "open source & bottom up" which don't take a hollistic view of the whole problem space
    * There are two camps, from user interviews: 
        * folks who are steeped in CD culture
        * folks who have a loose grasp on what CD means but need some help understanding how to get value from it or get from where they are to where they need to be
    * The work will be to define the common patterns used in pipelines
    * The MLOps space, as an example, is not very well connected to traditional CD pipelines.
        * https://github.com/cdfoundation/sig-mlops/blob/master/roadmap/2021/MLOpsRoadmap2021.md

### July 7, 2022

#### Participants
* Justin Abrahms, eBay
* Kara de la Marck, CDF
* Melissa McKay, JFrog
* Andrea Frittoli, IBM
* Ann Marie Fred, Red Hat
* \<AddMe\>

#### Agenda and Notes
* Introduction - Justin Abrahms, new Co-Chair
* Presentation - Uffizzi by Josh Thurman
    * on demand environments in k8s
    * designed to work with any ci/cd platform
    * triggered by cd events (maybe also CDEvents??)
    * QUICK LINKS-
        * Open Source Repo https://github.com/UffizziCloud/uffizzi_app
        * Public Road Map https://github.com/UffizziCloud/roadmap
        * GHA https://github.com/UffizziCloud/preview-action
        * Uffizzi  https://uffizzi.com/
        * Docs https://docs.uffizzi.com.  https://github.com/UffizziCloud/docs
        * Uffizzi Users Slack https://uffizzi.slack.com/join/shared_invite/zt-ffr4o3x0-J~0yVT6qgFV~wmGm19Ux9A#/shared-invite/email
        * Uffizzi Helm Chart https://artifacthub.io/packages/helm/uffizzi-app/uffizzi-app
        * Uffizzi Newsletter Sign-up. http://eepurl.com/hsws0b
* Open Action Items
    * Justin: intent based pipelines article
    * Melissa: Determine WHERE in the best practices site to add vocabulary documentation (https://bestpractices.cd.foundation/); Review Terry's suggestions from last meeting
    * Fatih & Ann Marie: address vocabulary split and conflicts in outstanding PRs - move to early-August meeting
* CDEvents and Pipeline terminology alignment (if time permits) - move to early-August meeting

### June 16, 2022

#### Participants
* Melissa McKay, JFrog
* Kara de la Marck, CDF
* Andres Almiray
* Josh Thurman
* Jeremy Adams
* Maria Ashby
* Richard Kilmurray
* Fatih Degirmenci
* Andrea Frittoli
* Brett Smith
* \<addme\>

#### Agenda and Notes
* Presentation - dagger.io by Jeremy Adams
* Open Discussion

### June 2, 2022

#### Participants
* Melissa McKay, JFrog
* Kara de la Marck, CDF
* Ann Marie Fred, Red Hat
* Jeremy Adams, Dagger
* Justin Abrahms, eBay
* Emil Bäckmark, Ericsson
* Fatih Degirmenci
* \<addme\>
    
#### Agenda and Notes
* Action Item Review, All
    * Jeremy Adams, Dagger.io - June 16th scheduled presentation
* SIG Interoperability Co-chair nominations/elections
    * NOMINATION: Justin Abrahms, eBay
* Ann Marie has [a talk repping this sig](https://drive.google.com/file/d/1UoufcCfqYzcBsD2zUDaKPg9V3BBFTF4g/view?usp=sharing) next week at cdCon virtual ([sched session link](https://cdcon2022.sched.com/event/12vF9/virtual-session-continuous-integration-and-continuous-delivery-pipelines-for-beginners-and-managers-ann-marie-fred-red-hat)) and OpenInfra Summit Berlin!
* [CDEventsCon wrap up blog post](https://cd.foundation/blog/2022/05/25/cdeventscon-2022-wrap-up/), including link to YouTube channel to all the talks and presentations at CDEventsCon
* **ACTION ITEM:** Fatih & Ann Marie address vocabulary split and conflicts in outstanding PRs
* **ACTION ITEM:** Melissa - Determine WHERE in the best practices site to add vocabulary documentation (https://bestpractices.cd.foundation/); Review Terry's suggestions from last meeting
* **ACTION ITEM:** Melissa & Justin finish up article next week at cdCon


### April 21, 2022

#### Participants
* Fatih Degirmenci, Ericsson Software Technology
* Kara de la Marck, CDF
* Melissa McKay, JFrog


#### Agenda and Notes
* Action Item Review, All
    * **ACTION ITEM:** Melissa still needs to reach out to dagger.io
    * **ACTION ITEM:** Justin/Melissa - wrap up intent driven pipeline thoughts for article
* SIG Interoperability Co-chair nominations/elections
    * Look for email in the mailing list and submit your nominations!
* Documentation Consult with Best Practices SIG - Terry Cox & Tara Hernandez
    * Web site in development: [https://deploy-preview-4--preview-site-cdf-bp.netlify.app/](https://deploy-preview-4--preview-site-cdf-bp.netlify.app/)
    * Consider audience - our current documentation is geared toward a more technical and implementation level
        * Step 1: link our current reference docs as they are in resources/references section
            * Keep our own copy for updates and maintenance in our own repo
            * Update the publication on Best Practices site periodically
            * **ACTION ITEM:** Kara to link intial resource docs
        * Consider higher level audience documentation (less detail)
            * What is the problem you are trying to solve???
            * **ACTION ITEM:** Fatih will work on higher level documentation
* Discussion about maturity models
    * [SLSA](https://slsa.dev/)
    * DORA metrics
    * Be careful about making value judgements based on maturity/effectiveness levels
* \<addme\>

### April 7, 2022

#### Participants
* Melissa McKay, JFrog
* Fatih Degirmenci, Ericsson Software Technology
* Mattias Linnér, Ericsson
* Justin Abrahms, eBay
* \<addme\>

#### Agenda and Notes
* Action Item Review, All
* Open PR Reviews
    * [Pipeline step types proposal](https://github.com/cdfoundation/sig-interoperability/pull/81)
    * [Initial proposal for pipeline stage terminology](https://github.com/cdfoundation/sig-interoperability/pull/76)
    * ACTION ITEM: Fatih pinging all involved to resolve all items between now and next meeting, open issues where needed
* Open Discussion
    * [What quality gates do you have?](https://github.com/cdfoundation/sig-interoperability/discussions/83)
    * ACTION ITEM: Justin - begin composing documentation on Quality Gates (from discussion material)
* Documentation considerations
    * Sync with Best Practices
    * Consider using HackMD
    * Split up the documentation resulting from most recent PRs into high level vs technical implementation details
    * ACTION ITEM: Melissa - reach out to Best Practices SIG on documentation (invite to meeting)
* New Discussion
    * [Slack thread (in general channel)](https://cdeliveryfdn.slack.com/archives/CJQU6EHHP/p1648923213508359)
    * [Intent-based pipelines](https://github.com/cdfoundation/sig-interoperability/discussions/91)
        * dagger.io
        * take a look at (for inspiration): 
          -  [shipa](https://shipa.io/miscellaneous/kubernetes-dagger-deployment-with-shipa/)?
          -  [Crossplane & Kubernetes Workshop](https://devrel.shipa.io/cp-idp-workshop)
          -  [Jenkins X](https://jenkins-x.io/blog/2020/11/11/accelerate-tekton/)
    * ACTION ITEM: Melissa - reach out to dagger.io for a possible presentation, come up with CI yaml (ideal example)
    * ACTION ITEM: Justin - work on blog post about intent based pipelines (the high level concept)
* \<addme\>

### March 17, 2022

#### Participants
* Melissa McKay, JFrog
* Mattias Linnér, Ericsson
* Mike Beemer, Dynatrace
* Fatih Degirmenci, Ericsson Software Technology
* \<addme\>

#### Agenda and Notes
* Action Item Review, All
* Meeting time change
    * Meeting time change to 15:00 UTC to match up with seasonal time changes
    * Melissa will update on the public calendar
* Presentation on the Open Feature Project by Michael Beemer
    * Open standard for feature flag management
    * https://open-feature.github.io/\<addme\>
* \<addme\>

### March 3, 2022

#### Participants
* Kara de la Marck, CDF
* Fatih Degirmenci, Ericsson Software Technology
* Justin Abrahms, eBay
* Mattias Linnér, Ericsson
* Melissa McKay, JFrog
* Ann Marie Fred, Red Hat

#### Agenda and Notes
* Action Item Review, All
* [cdCon](https://events.linuxfoundation.org/cdcon/) Updates, CFP, Kara de la Marck
* SIG Interoperability Co-chair nominations/elections
    * Melissa McKay has been nominated as new SIG Interoperability Chair and has accepted! Welcome Melissa McKay! 🎉
* Pipeline [Steps](https://github.com/cdfoundation/sig-interoperability/pull/81)/[Stages](https://github.com/cdfoundation/sig-interoperability/pull/76)/[Quality Gates](https://github.com/cdfoundation/sig-interoperability/discussions/83) and Software Supply Chain, All
    * [CNCF Security TAG Software Supply Chain Best Practices](https://github.com/cncf/tag-security/blob/main/supply-chain-security/supply-chain-security-paper/CNCF_SSCP_v1.pdf)
    * [Secure Software Factory RFC](https://docs.google.com/document/d/15M_Mzfqy634E_sqoslmOXsZJl4TedpbXpBjOfz-hnXk/edit#)
    * [SLSA](https://slsa.dev/)
    * [in-toto](https://in-toto.io)
* Pipeline certification/badge discussion
    * SRE, DevOps, Quality criteria
    * [Operate First](https://www.operate-first.cloud/)
* [Flow Framework](https://flowframework.org/)

### February 17, 2022

#### Participants
* Kara de la Marck, CDF
* Fatih Degirmenci, Ericsson Software Technology
* Anders Eknert, Styra
* Jeremy Stanley, OpenDev/Zuul
* Melissa McKay, JFrog
* Mattias Linnér, Ericsson
* Justin Abrahms, eBay
* \<addme\>

#### Agenda and Notes
* Action Item Review, All
* SIG Interoperability Co-chair nominations/elections, Fatih Degirmenci, All
* [cdCon](https://events.linuxfoundation.org/cdcon/) Updates, CFP, Kara de la Marck
    * cdCon CFP is open until midnight 18 February -- TOMORROW!!: https://events.linuxfoundation.org/cdcon/program/cfp/#overview
        - Please submit a talk even if you don’t know if your company is sponsoring travel yet. 
        - We do ask that speakers be at cdCon in person and present their talks live at cdCon.
    * If you think you may attend cdCon and would like to participate in a CDEvents Contributor Summit, [please fill out this form](https://docs.google.com/forms/d/e/1FAIpQLSeZGMEGldtkrj1viMcT9nQgAgHZVkIlzQZ45aTvN74992Mawg/viewform?usp=sf_link)
        * For each Contributor Summit, we should normally be able to provide breakfast, snacks at breaks, and beverages throughout the day. :coffee: :croissant:  
        - So it is important for CDF to have an estimate of number of attendees
* CDEvents 
    * Repo: https://github.com/cdevents
    * CDEvents logo finalised: https://github.com/cdfoundation/artwork/tree/main/cdevents
    * CDEvents website (beta): https://cdevents.dev/
    * CDEvents are on the landscape 😄  https://landscape.cd.foundation/
    * And on CDF website, listed with all the other projects  https://cd.foundation/projects/
* KubeCon update: CDEvents will have a full day co-located at KubeCon EU 🥳 
    * https://github.com/cdfoundation/sig-events/issues/115
    * This will be officially announced soon. If you will be at [KubeCon EU](https://events.linuxfoundation.org/kubecon-cloudnativecon-europe/) please do join us!
* Discussion on Quality Gates:
    * GH Discussion: https://github.com/cdfoundation/sig-interoperability/discussions/83
    * Anders Eknert, from Styra, is joining us to discuss quality gates.


### February 3, 2022

#### Participants
* Kara de la Marck, CDF
* Justin Abrahms, eBay
* Oliver Nocon, SAP
* fungi
* \<addme\>

#### Agenda and Notes
* Action Item Review, All
* [cdCon](https://events.linuxfoundation.org/cdcon/) Updates, CFP, Kara de la Marck
    * cdCon CFP is open until midnight 18 February: https://events.linuxfoundation.org/cdcon/program/cfp/#overview
        - Please submit a talk even if you don’t know if your company is sponsoring travel yet. 
        - We do ask that speakers be at cdCon in person and present their talks live at cdCon.
        - However, restrictions are loosening around the world and travelling to cdCon will likely be possible for most individuals (although regretably maybe not for all)
    * We are currently organising the Contributor Summits for cdCon 2022. 
        * The Contributor Summits are focused on CDF projects: https://cd.foundation/projects/
        * For all CDF projects that are interested in hosting a Contributor Summit at cdCon, please appoint a lead organiser/host for your summit and have that individual fill out the form below:
 https://docs.google.com/forms/d/e/1FAIpQLSfJGFdQhFAbScBt3y3sW0WCQMl903X9T3ycmix0PpB2Zq8aoQ/viewform
        * The deadline to fill out the form and formally request space at cdCon is February 28.
        * For each Contributor Summit, we should normally be able to provide breakfast, snacks at breaks, and beverages throughout the day. :coffee: :croissant:
* Fosdem is this weekend!! https://fosdem.org/2022/
    * [CI/CD devroom](https://fosdem.org/2022/schedule/track/continuous_integration_and_continuous_deployment/)
* SIG Interoperability Co-chair nominations/elections, Fatih Degirmenci, All
* New work around terminology for pipeline [stages](https://github.com/cdfoundation/sig-interoperability/pull/76) and [steps](https://github.com/cdfoundation/sig-interoperability/pull/81) - see links to PRs. Ann Marie Fred
* Updating SIG Interoperability Roadmap, Reminder
    * Link to the document: https://docs.google.com/document/d/1uf3sb-WJUp3Acd3WYL5SvgVECHevonufJOxd6KftOxc/edit#
    * Software Supply Chain
        * Standardized Metadata
        * Artifact Handling
        * Policy Driven CD
    * CDEvents 
    * Would be interesting to outline or create a catalogue of quality gates. 
        * Gather a list of what quality gates companies and teams are using in the wild. 
            * Mini case studies for different quality gates would be interesting.
            * How to gather: Survey? Shoutout on channels? See action items below.
            * Relates to best practices
            * Also, would be interesting to consider how to evaluate pipelines (not testing the actual pipeline or security concerns, necessarily), but really what should a pipeline contain. Again, very much a best practices question.
            * What signals do we use for quality?
                * execution speed of pipelines, etc
                * How many quality checks, ideal range
                * how do the quality checks bucket -- interesting to see if this becomes evident once catalogue created (eg, gates in place pre and post production/rollout)
* \<addme\>

#### Action Items
* [Justin Abrahms to create discussion on Interop SIG repo on what quality gates on being used by teams.](https://github.com/cdfoundation/sig-interoperability/discussions/83)
* Kara to make sure CDF publicizes the discussion.
* Kara to bring in others, from Styra, etc, to discuss how they see quality gates being used in practice.

### January 20, 2022

#### Participants
* Fatih Degirmenci, Ericsson Software Technology
* Kara de la Marck, CDF
* Jeremy Stanley, OpenDev/Zuul
* Ann Marie Fred, Red Hat
* Emil Backmark, Ericsson
* Mattias Linnér, Ericsson
* Jalander Ramagiri, Ericsson Software Technology
* Ramin Akhbari, Salesforce
* Erik Sternerson, doWhile
* Justin Abrahms, eBay

#### Agenda and Notes
* Action Item Review, All
* cdCon Updates, CFP, Kara de la Marck
    * cdCon CFP is open: https://events.linuxfoundation.org/cdcon/program/cfp/#overview
        - Suggestion from Kara is to submit a talk even if we don’t know if we’re allowed to travel yet
* SIG Interoperability Co-chair nominations/elections, Fatih Degirmenci, All
* Open Infra Summit Berlin, Jeremy Stanley
    * CFP for upcoming Open Infra Summit is open
    * There is a CI/CD track as part of summit
    * CFP is available here: https://cfp.openinfra.dev/app/berlin-2022
* SupplyChainSecurityCon
    * It will be colocated in Open Source Summit NA
    * CFP is available here: https://events.linuxfoundation.org/open-source-summit-north-america/about/supplychainsecuritycon/
* New work around terminology for pipeline [stages](https://github.com/cdfoundation/sig-interoperability/pull/76) and [steps](https://github.com/cdfoundation/sig-interoperability/pull/81) - see links to PRs. Ann Marie Fred
* Updating SIG Interoperability Roadmap, Reminder
    * Software Supply Chain
        * Standardized Metadata
        * Artifact Handling
        * Policy Driven CD
    * Events
    * Link to the document: https://docs.google.com/document/d/1uf3sb-WJUp3Acd3WYL5SvgVECHevonufJOxd6KftOxc/edit#
* \<addme\>

#### Action Items
* \<addme\>