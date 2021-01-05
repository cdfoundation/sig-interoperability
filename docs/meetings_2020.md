# CDF Interoperability SIG Meetings 2020

[![HacmKD documents](https://hackmd.io/badge.svg)](https://hackmd.io/niM1USFoQyycav8IczCmzQ?edit)

## Note

This document contains the minutes of the SIG Interoperability meetings held during 2020 and kept for historical/archive purposes.
Please do not edit this document.

If you are looking for the latest SIG Interoperability minutes of meetings, please head over to [CDF Interoperability SIG Meetings document](https://hackmd.io/HuufSDMaTPyb3qxkyBKg3A?view).

## Quick links

* [Logistics](#Logistics)
* [Meeting Recordings](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG)
* [Agenda and Notes](#Agenda-and-Notes)
    * [2020-12-10 Meeting](#December-10-2020)
    * [2020-11-26 Meeting](#November-26-2020)
    * [2020-11-12 Meeting](#November-12-2020)
    * [2020-10-29 Meeting](#October-29-2020)
    * [2020-10-15 Meeting](#October-15-2020)
    * [2020-10-01 Meeting](#October-1-2020)
    * [2020-09-17 Meeting](#September-17-2020)
    * [2020-09-03 Meeting](#September-3-2020)
    * [2020-08-20 Meeting](#August-20-2020)
    * [2020-08-06 Meeting](#August-6-2020)
    * [2020-07-23 Meeting](#July-23-2020)
    * [2020-07-09 Meeting](#July-9-2020)
    * [2020-06-25 Meeting](#June-25-2020)
    * [2020-06-11 Meeting](#June-11-2020)
    * [2020-05-28 Meeting](#May-28-2020)
    * [2020-05-14 Meeting](#May-14-2020)
    * [2020-04-30 Meeting](#April-30-2020)
    * [2020-04-16 Meeting](#April-16-2020)
    * [2020-04-02 Meeting](#April-2-2020)
    * [2020-03-19 Meeting](#March-19-2020)
    * [2020-03-05 Meeting](#March-5-2020)
    * [2020-02-20 Meeting](#February-20-2020)
    * [2020-02-06 Meeting](#February-6-2020)
    * [2020-01-23 Meeting](#January-23-2020)

## Logistics

* Meeting notes on HackMD.io: https://hackmd.io/@cdf-sig-interoperability/ry3TTB5DL
* When: every even week on Thursdays at 16:00UTC (*See your timezone [here](https://time.is/1600_in_UTC)*).
* Zoom Bridge: https://zoom.us/j/827082528?pwd=RlN5OUZtVVBuZGZRY0NBRnZyZ0NJQT09
* Zoom International dial-in numbers: https://zoom.us/zoomconference
* Meeting Recordings: [CDF Youtube Channel SIG Interoperability Playlist](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG)
* CDF Public Calendar: [here](https://calendar.google.com/calendar/embed?src=linuxfoundation.org_mhf0kmgedn67ihni8r129avp24%40group.calendar.google.com&ctz=America%2FLos_Angeles)
* Past Presentations in CDF Presentations Repository: https://github.com/cdfoundation/presentations/tree/master/sig-interoperability
* Presentation Schedule: https://docs.google.com/document/d/1Owg_I52WEXzqF8g_lX6OTdwbHkH4Z2-7TBA7eCSVMqY/edit

### December 10, 2020

#### Participants
* Andreas Grimmer (Dynatrace)
* Tracy Ragan (DeployHub)
* Dave Sudia (GoSpotCheck)
* Mattias Linnér (Ericsson)
* Emil Bäckmark (Ericsson)
* James Rawlings (CloudBees)
* Steve Taylor (DeployHub)
* Oliver Nocon (SAP)
* Andrea Frittoli (IBM)
* Fatih Degirmenci (Ericsson Software Technology)
* James Strachan (CloudBees)
* Tracy Miranda (CDF)

#### Agenda and Notes
* Action Item Review, All 
* Upcoming SIG Meetings
    * Propose to cancel meeting on December 24 and reconvene on January 7th
    * We meet January 7th
    * SIG Interoperability meets 1st and 3rd Thursdays every month
* Wrapping up [Interoperability Whitepaper](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit), All
    * Waiting for creative team to finalize the work with annual reports
* Events in CI/CD Workstream to become a separate SIG, Workstream Members
    * See the [workstream meeting minutes](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w?view) for details
    * EB: The topic was brought up during workstream meetings by Tracy Ragan to increase the visibility and attract more people by making it a SIG
    * EB: The question of how to relate Events in CI/CD SIG to Interoperability SIG if/when it becomes one
    * EB: The topic will be brought up to CDF TOC on January 19th
    * TR: Events is a topic in CNCF as well and having Events in CI/CD a SIG would help with collaboration and cross pollination
    * TM: What's the scope of the discussion within the events workstream?
    * EB: Focusing on events.
* [Standardized Metadata](https://hackmd.io/BYbkuR8uSlKt_w7Y4KE1OQ), James Strachan, All
    * JS: We could perhaps start simple with a file. We went with CRD on Kubernetes.
    * JS: Getting as many examples as we can find is important such as Tekton Chains, Ortelius, eBay to find similarities.
    * JS: Starting with something simple and obvious such as what's Git Commit SHA, Repo Url.
    * JS: Over time, other things could be looked into such as test metadata.
    * JS: There is [TAP](https://testanything.org/) to describe test results. GitHub Actions use TAP to describe test results. 
    * JS: If this becomes something, we could have some CDF CRD or just schema document to make it consumable by anything - CRD, file, events.
    * JS: Starting simple. If we can't agree on everything, we can start with parts of it such Git Commit or Issues or Test Results etc to reach consensus on certain things quickly.
    * JS: Splitting metadata to chunks and work on them in parallel, treating them separate metadata.
    * JS: Start a new repo on CDF and try things out. Generate simple structure to experiment with things. Collect all the examples. Work on them collaboratively.
    * JR: There are many tools out there to help with keep iterating, reviewing, working together.
    * TR: Ortelius team would be interested in this since this is one of the areas the team is looking into.
    * JR: The end goal is interoperability and this is exciting.
    * TR: The goal of Ortelius is central CMDB for microservices (or any type of component). Should we be tracking metadata generated by Argo or Spinnaker and what? Where do we draw the line.
    * ST: One of the things we should look at is SPDX. There is a lot of specification we can grab and roll up to the release and deployment.
        * [SPDX Package Specification](https://spdx.github.io/spdx-spec/3-package-information/)
        * [SPDX Relationship Specification](https://spdx.github.io/spdx-spec/7-relationships-between-SPDX-elements/)
    * EB: We use Eiffel events to handle concepts of activities, artifacts, test results in Ericsson as an example.
        * [Eiffel Protocol](https://github.com/eiffel-community/eiffel) with a vocabulary for metadata
    * ST: We start with a small subset and cover more over time. Starting with SHA/commit for example and extending over time.
    * FD: Artifacts could be the other thing we could look at.
    * ST: There could be other commonalities here as well. Starting at the top for example name and version number. Naming/terminology could be the tricky thing - what is artifact? Could be a similar work to Rosetta Stone we have.
    * ST: SPDX is The Software Package Data Exchange
* CDF End of the year party
    * December 15th - noon est coast time - bring your own beer and donuts
* [Ortelius](https://github.com/ortelius/ortelius) Presentation/Demo, Tracy Ragan, Steve Taylor (2nd January Meeting 1/21)

#### Action Items
* Fatih to ping Cameron on Jenkins Spinnaker for whitepaper
* Ramin A to bring an example manifest from eBay for metadata topic
* Tracy R/Steve T to demo Ortelius (manifest/metadata/visibility focused)
* ~~James S to bring Jenkins X metadata example to standardized metadata discussion~~
* Events in CI/CD workstream to provide input to standardized metadata topic based on their discussions
* Tracy M to bring the whitepaper to the attention of CDF creative team
* Tracy M to help with updating meeting invitation according to what is agreed
* Tracy M to help with creation of a repo for standardized-metadata
* Steve to start the work on commit metadata
* Dave to start the work on artifact metadata
* Emil to b bring Eiffel example in new repo
* Steve/Tracy R to bring Ortelius example in new repo

#### Meeting Recording
* \<addme\>

### November 26, 2020

#### Participants
* Andreas Grimmer (Dynatrace)
* Fatih Degirmenci (Ericsson Software Technology)
* James Rawlings (CloudBees)
* Oliver Nocon (SAP)
* Kara de la Marck (CloudBees)
* Emil Bäckmark (Ericsson)
* Mattias Linnér (Ericsson)
* James Strachan (CloudBees)
* Vibhav Bobade (Red Hat)
* Tracy Miranda (CDF)

#### Agenda and Notes
* Action Item Review, All 
* [Interoperability Whitepaper](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit), All
    * TM: Keep the whitepaper in line with CDF way of expressing things such as CD, Pipeline Orchestration
    * Updates to the chapters
        * What are we discussing with Continuous Delivery?
        * What Does Interoperability Mean in Continuous Delivery context?
        * Key Considerations, Constraints, and Concerns
        * Trends
            * Reusable Libraries
            * Standardized Metadata
    * New Case Studies
        * Tekton Client for Jenkins
        * Jenkins X and Tekton
        * Zuul
    * Questions and Open Issues
        * Addressing different audiences
            * Decision makers: Should we have an Executive Summary???
        * References need to be gathered at the end
        * Contributors are listed based on history of the doc (people contributed case studies/chapters and commented)
        * New Chapters added during last meeting
            * APIs
            * Secrets
        * Future and conclusion still missing
* [Standardized Metadata](https://hackmd.io/BYbkuR8uSlKt_w7Y4KE1OQ), All

#### Action Items
* ~~Fatih to ping Vibhav on Jenkins Tekton Plugin for whitepaper~~
* Fatih to ping Cameron on Jenkins Spinnaker for whitepaper
* ~~Tracy M to arrange a working session for the whitepaper~~
* ~~Tracy M to update the meeting time to 16:00UTC~~
* Ramin A to bring an example manifest from eBay for metadata topic
* Tracy R/Steve T to demo Ortelius (manifest/metadata/visibility focused)
* James S to bring Tekton metadata example to standardized metadata discussion
* Events in CI/CD workstream to provide input based on their discussions
* Tracy M to bring the whitepaper to the attention of CDF creative team

#### Meeting Recording
* https://www.youtube.com/watch?v=QpQAy_E0kLg

### November 12, 2020

#### Participants
* Fatih Degirmenci, Ericsson Software Technology
* James Rawlings, CloudBees
* Jeremy Stanley, OIF/Zuul
* Mattias Linnér, Ericsson
* Kara de la Marck, CloudBees
* Tracy Miranda, CDF
* Andrea Frittoli, IBM
* Emil Bäckmark, Ericsson
* Oliver Nocon, SAP

#### Agenda and Notes
* Action Item Review, All
* Meeting time for SIG Interoperability, All
    * TM: New time makes it challenging for community members from NA to join
    * TM and Fatih: Move meeting one hour later in UTC time (16:00 UTC). Discussion: agreement. Time may move again for summer time changes. 
* [Interoperability Whitepaper](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit), All
    * TM: Would be good to give context on size of deployments, esp for case studies
    * Kara: should we have section on APIs/Standards/Open Standards?
    * Tracy: Open Standards are likely what we are working towards. :)
    * APIs section good -- Lighthouse uses same APIs as Prow, as an example with CRDs, Tekton, Kubernetes also good examples
    * New/additional case studies
    * Remaining chapters
* [Standardized Metadata](https://hackmd.io/BYbkuR8uSlKt_w7Y4KE1OQ), James Strachan, All
    * Meeting and workstream setup
    * We parked the topic until we have more people
* [Ortelius](https://github.com/ortelius/ortelius) Presentation/Demo, Tracy Ragan, Steve Taylor
    * This presentation will probably happen on December 10th
* SIG Best Practices
    * This SIG is getting started and the first meeting will take place on Monday, November 16. Please check CDF Public Calendar.
    * The SIG takes Accelerate book as the starting point.
    * Reach out to Tracy Miranda if you want to be included in the invite.

#### Action Items
* Fatih to ping Vibhav on Jenkins Tekton Plugin for whitepaper
* Fatih to ping Cameron on Jenkins Spinnaker for whitepaper
* Tracy M to arrange a working session for the whitepaper
* Tracy M to update the meeting time to 16:00UTC
* ~~Fatih D to create HackMD document for the metadata work~~: https://hackmd.io/BYbkuR8uSlKt_w7Y4KE1OQ
* ~~Fatih D sync with Oliver on case study for whitepaper~~
* Ramin A to bring an example manifest from eBay for metadata topic
* Tracy R/Steve T to demo Ortelius (manifest/metadata/visibility focused)
* ~~James S to store slides on https://github.com/cdfoundation/presentations~~: https://github.com/cdfoundation/presentations/pull/37

#### Meeting Recording
* https://www.youtube.com/watch?v=EH9NAEoWdNI

### October 29, 2020

#### Participants
* Ramin Akhbari (eBay)
* Fatih Degirmenci (Ericsson Software Technology)
* Nitin
* Steve Taylor (DeployHub)
* Tracy Ragan (DeployHub)
* Christie Wilson (Google)
* Mattias Linnér (Ericsson)
* James Rawlings (CloudBees)
* James Strachan (CloudBees)
* Vibhav Bobade (RedHat)
* Jerop Kipruto (Google)
* Sacha Wharton
* Jithin Emmanuel (Verizon Media)
* Tracy Miranda (CDF)
* Oliver Nocon (SAP)
* Emil Backmark (Ericsson)
* Kara de la Marck (CloudBees)

#### Agenda and Notes
* Action Item Review, All
* Daylight Saving Time ends, Fatih Degirmenci
    * https://time.is/compare/1500_12_Nov_2020_in_UTC/PT/CT/ET/CET/China
* Feedback from [ICST2020 CI/CD Industry Workshop](https://conf.researchr.org/home/cciw-2020), Fatih Degirmenci
    * FD: One of the things raised was availability of *maturity model* so companies could measure themselves against it and whether CDF has something on this
    * TM: CDF will start a best practices working group. Things will be based on Accelerate Book.
    * TM: Something that's easy to understand and it may not be called *maturity model*.
    * FD: The other one was what is continuous/integration/delivery/deployment which we are already working on so we are on the right path here
    * FD: Standardization was another question
    * FD: How to get some collaboration going on between academia, industry, and communities which i pointed them to CDF
    * TM: Academia can be associate members of the CDF.
    * FD: https://sites.google.com/site/gjournalclub/
    * FD: https://groups.google.com/forum/#!forum/google-journal-club
    * FD: Tracy Miranda is meeting with the group leaders
* Standardized Metadata, James Strachan
    * JS: There was a conversation around this topic last couple of years
    * JS: We have been doing releases but never discussed having common metadata
    * JS: We can start writing a spec and then look at integrating into Jenkins X, Tekton, etc.
    * ML: How to transport the metadata vs how to define metadata?
    * JS: Initial focus was on defining metadata. Looks like CRD but it doesn't have to be CRD.
    * JS: It could be a message, it could be yaml.
    * JS: Once we agree on metadata, we could look at more.
    * JS: It doesn't have to be custom resource - it could be a file, URL, message bus.
    * JS: Lets start with spec/schema, examples. First thing is to start generating this data.
    * JS: Eventually the tooling to discover this metadata. We can start baking the metadata in.
    * JS: Start defining metadata first, see what's common between Spinnaker, etc. THere is overlaps with Helm.
    * JS: There is also app spec in Kubernetes world which may be good to align.
    * JS: We should be able to come up with common/simplish stuff - git sha, url to pipeline log, etc.
    * RA: Are you advocating for application metadata standard or release metadata standard.
    * JS: Bit of both. Basic idea is what could we bake for the consumers doing CD to make it possible to understand what happens going further.
    * JS: It is good to give people information about what to choose and allow automation so people don't need to click buttons.
    * RA: eBay created concept of a manifest to list what got deployed. Everything about what's got deployed in the manifest.
    * RA: Quality gates themselves are associated with the manifest and include series of badges. 
    * RA: Number of badges: Unit test pass, Integration test pass, security scan pass, etc so admission controller allows what gets deployed.
    * RA: An object that encompases all the information about a release?
    * JS: Yes.
    * RA: Concept of release manifest?
    * ST: Ortelius project has manifest defining what release has and it is stored in the DB.
    * ST: When you are dealing with microservices, you end up with many of them. You need to associate them with applications.
    * ST: Using pointers to data instead of having the data in the manifest.
    * ST: There is a standard on packages, allowing tracking back. (name??)
    * CW: There is a Tekton project called "Chains" (https://github.com/tektoncd/chains). in-toto is working on a standard around Software supply chain protection. (https://in-toto.io/specs/)
    * JS: Adding link is good.
    * RA: Once you have an object which encapsulates basic data about what is being released (release manifest at eBay), this opens up possibilities.
    * ST: Is the manifest object immutable?
    * RA: Once the object is created, it is immutable. You do not modify manifest.
    * RA: If changes are required, you go through the automated process to get new one created.
    * RA: I can grab the pieces going there bring to this group. (combination of data - dependencies, git repo, etc.).
    * TR: We've been asked to add additional data into Ortelius. (hermetic manifest/helm chart)
    * JS: Starting with discovery, strawman doc
    * Tracy Miranda, James Strachan, Steve Taylor volunteer
    * Everyone to share the problems, ideas, etc.
* [CI/CD Interoperability Whitepaper](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit), All
    * Time plan for CI/CD Interoperability Whitepaper
        * TM: Synched with the creative team and received some guidelines, CDF Template, looks straightforward
        * TM: Decide on some diagrams.
        * TM: Aim to get this done before end of the year.
        * TM: End of November is the target date to get to the creative team.
    * Any other case studies coming in?
        * FD: Oliver from SAP
* Waypoint
    * Tracy M to make introductions
* Jenkins X and Tekton Integration Demo, James Rawlings, James Strachan
    * The recording will be available on Youtube CDF Channel

#### Action Items
* Fatih D to create HackMD document: https://hackmd.io/BYbkuR8uSlKt_w7Y4KE1OQ
* Fatih D sync with Oliver on case study for whitepaper
* Ramin A to bring an example manifest from eBay for metadata topic
* Tracy R/Steve T to demo Ortelius (manifest/metadata/visibility focused)
* James S to store slides on https://github.com/cdfoundation/presentations
* ~~Tracy M to come up with proposed time plan for interop whitepaper~~
* ~~Fatih D to add "metadata" topic to next meeting~~

#### Meeting Recording
* https://www.youtube.com/watch?v=E_EuPAdhnqM

### October 15, 2020

#### Participants
* Emil Bäckmark, Ericsson
* Fatih Degirmenci, Ericsson Software Technology
* Tracy Miranda, CDF
* Tracy Ragan, DeployHub
* Christie Wilson, Google
* James Rawlings, CloudBees
* Dave Sudia (GoSpotCheck)
* Cameron Motevasselani (Armory)
* James Strachan, CloudBees
* Oliver Nocon, SAP

#### Agenda and Notes
* Action Item Review, All
* Reflections from [cdCon](https://events.linuxfoundation.org/cdcon/), All
    * TM: There were many people with questions like what is CD.
    * TM: First event online, community coming together
    * TM: Intereactive sessions were received well
    * TM: Some Tekton talks were great and A.Frittoli's talk was best talk
    * TM: To summarize, it was great
    * TM: 1354 registrants, 70% of them accessed to the platform, 200 first day, 150 second day
    * TM: Full report will be available soon
    * TM: Recordings from cdCon should be available soon (starting on 22nd October). BoF reconrdings will not be available
    * JR: Lots of people were involved in Jenkins BoF.
    * JS: Next time, we could have more generic talks/none-specific to projects. (e.g. how do you do version control, GitOps) for practicioners to debate on.
    * JS: Having broader BoF would allow people to discuss general issues.
    * EB: Interop BoF was some kind of general session.
    * Conflicts in the schedule made things tricky.
    * TR: Chatrooms like experts chatroom, speaker chatroom, general chatroom to enable discussions.
    * EB: Chatrooms could be kept open during the entire summit.
    * JR: Slack/Discourse like platform may be good to think about. 
    * TR: On existing slack, cdCon area/channel would be interesting for people to join.
    * TM: KubeCon people encourage people to have them on Slack to keep them engaged.
    * TM: How best structure expert/discussion chatrooms?
    * JR: User forum like thing. Bring your user story? What is your biggest issue/problem, what do you miss from the technology? Fellow users talking to each other.
    * TM: Planning for the next cdCon started. Probably in June 2021. North America and/or Europe. Contributor Summit for each project could help welcoming people. Any feedback on this, please reach out to Tracy.
    * EB: It was very late for people joining from Asia so having separate zones would help. Is it possible to run event longer.
    * DS: Another event was doing rebroadcast which could be an option.
* Time plan for the whitepaper
    * Decide on when to have the first draft
    * TM: I can check with creative folks to give feedback.
* [CI/CD Interoperability Whitepaper](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit), All
    * High Level Continuous Delivery Whitepaper document: https://docs.google.com/document/d/1aZT__F57g1BMPzpsV6RAC86k_FfetkAWMhdVT22PZrM/edit?ts=5f875eda#heading=h.rrar1dgps27e
    * Continuous Delivery Definitions work continue on: https://docs.google.com/document/d/1IUSmgtw5eC2JwyfiX7IPK3twl3MSjWAsmCKmJ6Y5z-w/edit#heading=h.yl0j54hk33l
    * Jenkins X and Tekton case study will be available soon. We should see something by the next meeting.
* CI/CD Industry Workshop, October 24
    * The workshop runs as part of ISCT 2020
    * https://conf.researchr.org/home/cciw-2020#program
* Any low hanging fruits
    * TM: Standardized metadata for testing (eg junit)
    * JS: Test results interop, Visualizing test results, commits, releases could be something, should we have canonical format.
    * EB: We are using events for this type of use case
    * JS: It would be nice if CDF could come with some kind of format which we all can write tools to generate/consume
    * JS: Starting simple and small could be really useful
    * CM: A lot of people look at canary deploys, etc. But testing is generally done on CI part. I would be interested in having standard format of testing.
    * ON: Collecting release information together would be good. Having some metadata would be helpful.
    * JS: Once we get started, we can decide if we should have standard way to collect. (eg. CDF released metadata thing)
* Topics for upcoming meetings
    * Metadata workstream?
    * James R & James S for Jenkins X and Tekton Integration demo?
    * Tracy R for Ortelius demo?
 
#### Action Items
* Tracy M to come up with proposed time plan for interop whitepaper
* Fatih D to add "metadata" topic to next meeting
* ~~Tracy M to add SIG BoF HackMD document to session~~ 
* ~~Christie and Cameron to move the CI/CD definitions section to the new doc and update the whitepaper draft with the link~~

#### Meeting Recording
* https://www.youtube.com/watch?v=5MBHiHxm_m0

### October 1, 2020

#### Participants
  - Andreas Grimmer (Dynatrace)
  - Fatih Degirmenci (Ericsson Software Technology)
  - James Rawlings (CloudBees)
  - Gareth Evans (CloudBees)
  - Emil Bäckmark (Ericsson)
  - Dave Sudia (GoSpotCheck)
  - Mattias Linnér (Ericsson)
  - Cameron Motevasselani (Armory)
  - Tracy Miranda (CDF)
  - James Strachan (CloudBees)

#### Agenda and Notes
  - Action Item Review, All
      - Tracy Miranda will start a new working group to focus on definitions
      - Reach out to Tracy if you are intersted to contribute
  - [cdCon](https://events.linuxfoundation.org/cdcon/), Tracy Miranda
      - Happening next week!
      - [Schedule](https://events.linuxfoundation.org/cdcon/program/schedule/)
      - TM: Registration is free and donations are optional so people can make donations.
      - TM: Changes were made to the program to accomodate different timezones such as Europe.
      - TM: Interactive sessions are added to the agenda such as Birds of a Feather sessions.
  - [cdCon SIG Interoperability Birds of a Feather Session](https://cdcon2020.sched.com/event/eicz), Tracy Miranda
      - [Looking for volunteers](https://docs.google.com/document/d/1U9Cp8Xoa-FqzL5UUUaCaEk3-9AeVQBB9qhPzLAvPmQI/edit#)
      - [Doc to keep BoF notes](https://hackmd.io/AizhDLlRTyuYWz-XidWdGg?view)
      - TM: A BoF Session for SIG Interoperability is scheduled.
      - TM: SIG participants are urged to join to the BoF, helping others.
  - [CI/CD Interoperability Whitepaper](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit), All
      - Definitions
          - TM: The conversations on definitions ignited the conversation around the need CDF to work on this area on a separate paper.
          - TM: The term CI/CD needs improving and we can perhaps focus on Continuous Delivery which CI can be considered as a component.
          - TM: A blog post was published on CDF Website. [Link to blog post](https://cd.foundation/blog/2020/09/24/we-need-to-stop-using-the-term-ci-cd/).
          - DS: Sizeable chunk of people think in CD terms but others fall back to CI/CD. Lack of consistency.
          - TM: Will have a keynote during cdCon and terms is one of the topics.
          - DS: This is something we need to work on together.
      - What does interoperability mean in CI/CD?
          - Review and work needed.
      - Trends - Events in CI/CD
          - AG: We worked on problem statement within the workstream and pointed events as something to investigate in our contribution to the whitepaper.
          - AG: We still have some wording/terminology issue. Any feedback is welcome!
          - EB: Looked at CNCF Landscape and noticed they use product vs project.
          - JR: Product is something from a company and project is something developed within community.
      - Case Studies
          - JR: Jenkins X native integration Tekton catalog could be a good contribution.
          - CM: We should have something for Spinnaker.
          - DS: Summarized the presentation given a month ago. Any feedback is appreciated.
          - EB: The contribution is under review and it will hopefully come before the next meeting.
          - TM: FinTech (Capital One) is pretty active in CDF.

#### Action Items
  - Tracy M to add SIG BoF HackMD document to session 
  - ~~Tracy M to followup Zoom Policy change, https://github.com/cdfoundation/foundation/issues/214~~
  - Christie and Cameron to move the CI/CD definitions section to the new doc and update the whitepaper draft with the link
  - ~~Tracy M will look at Christie's work and Tracy R's definitions.~~

#### Meeting Recording
  - https://youtu.be/Kwf8Nn6lPIA

### September 17, 2020

#### Participants
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Mattias Linnér (Ericsson)
  - Christie Wilson (Google)
  - Kara de la Mark (CloudBees)
  - Tracy Miranda (CDF)
  - Jeremy Stanley (OSF/Zuul)
  - Tracy Ragan (DeployHub)

#### Agenda and Notes
  - Action Item Review, All
      - This meeting's Zoom link on calendar is now updated -- thank you Tracy and Fatih.
      - Quick discussion on https://github.com/cdfoundation/foundation/issues/214
  - CI/CD Interoperability Whitepaper, All
      - Outline: https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit
      - Continue discussion on definition of Continuous Integration (not that contentious), and Continuous Delivery and Continuous Deployment (lots of discussion last week and on Whitepaper)
          - (Christie) Would like to suggest we use this separate doc to break down the definition before wordsmithing (https://docs.google.com/document/d/1IUSmgtw5eC2JwyfiX7IPK3twl3MSjWAsmCKmJ6Y5z-w/edit#)
          - Tracy M, Fatih: +1 
          - Christie: Should we have separate paper for definitions, so doesn't block this White Paper, and this one works from basis of Continuous Delivery containing all of the CI/CD practices under discussion.
          - Fatih: Keeping definitions is important for understanding interoperability in CI/CD
          - Ramin: Additional White Paper on definitions good idea
          - Tracy M, Tracy R: +1
          - Tracy R: Strong agreement. Stating this is what Continuos Delivery is and CDF address all of it.
          - Ramen: +1 This is how we think of Continuous Delivery at eBay
          - Tracy M: This is inline with Accelerate book. CD is umbrella of these different processes
          - Tracy R: Some of this work on definitions has been done, through process with ToC.
          - Fatih: Continuous Delivery then includes CI and Continuous Deployment. It is the umbrella term. Are we in agreement?
          - Ramin, Tracy R: Yes
          - Tracy M: Christie has been working on CI def, in reponse to questions raised by CDF Ambassadors
          - Christie: We should be able to have definitions that can be used to address question of 'Am I doing CI?' 
          - TR: We ned high level definitions. Definitions don't have to relate to a specific step in the process. Think in terms of higher level compliance requirements. Need to think in terms of goals for each of the steps. Benefit statements.
          - Tracy M: Proposal to start another white paper addressing definitions of these goals. [general support]
          - Tracy R: Doing a white paper on Continuous Delivery and its goals is important initiative
          - Fatih: to unblock the current White Paper skip the definitions here, and leave that to the other papers. Parallel White Paper on definitions makes a lot of sense. We will rename the current paper.
          - TOC CI/CD Definitions document: https://docs.google.com/document/d/1VpNd2v4SjjbOIiMylIlb8NVe_t7YdDVYYUgVUkGuOgg/edit?usp=sharing
          - CI/CD Definitions document - new: https://docs.google.com/document/d/1IUSmgtw5eC2JwyfiX7IPK3twl3MSjWAsmCKmJ6Y5z-w/edit#heading=h.yl0j54hk33l
      - Address: What Does Interoperability mean in CI/CD context?
      - Fatih, review of his notes. Ultimately, Interoperability in CI/CD is broadly in line with text book definition of interoperability -- enabling the exchange of data.

#### Action Items
  - Tracy M to followup Zoom Policy change, https://github.com/cdfoundation/foundation/issues/214
  - ~~Tracy R to find the document the TOC worked on early on the definitions of Continuous Integration/Delivery/Deployment~~
  - Christie to move the CI/CD definitions section to the new doc and update the whitepaper draft with the link
  - Tracy M will look at Christie's work and Tracy R's definitions.

#### Meeting Recording
  - \<addme\>

### September 3, 2020

#### Participants
  - Kara de la Marck (CloudBees)
  - Dave Sudia (GoSpotCheck)
  - Andreas Grimmer (Dynatrace)
  - Emil Bäckmark (Ericsson)
  - Cameron Motevasselani (Armory)
  - Ramin Akhbari (eBay)
  - Tracy MIranda (CDF)
  - Mattias Linnér (Ericsson)
  - \<addme\>

#### Agenda and Notes
  - Action Item Review, All
  - RA: Can we PLEASE get this meeting's zoom link in the invite?
  - TM: Yes! 
  - CI/CD Interoperability Whitepaper, All
      - [Draft](https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit)
      - Excellent additions on defining CI and CD by Christie Wilson, Cameron Motevasselani, and others. Discuss.
      - Cameron discusses his additions on CI CD definitions (see Whitepaper)
      - TM: Continuous delivery to include people aspect. Cameron agreement
      - EB: Continuous Deployment strictly speaking would end at deployment into production, but with recent tools providing canary and blue/green deployments and such to staging environments and sometimes also to production that definition doesn't really hold anymore. The border between Continuous Delivery and Continuous Deployment is more fuzzy now than earlier.
      - RA: https://semaphoreci.com/blog/2017/07/27/what-is-the-difference-between-continuous-integration-continuous-deployment-and-continuous-delivery.html Contains defitions on these terms that are widely seen as industry standards. C Delivery is process of automating everything. C Deployment means delivering value to customers, ie to production. If it's not that, then it's still C Delivery. Definition on CDF site should be updated.
      - DS: Cameron's definitions and what we are discussing is kind of the flip of that. So, C Delivery is the total delivery. C Deployment is deployment to different environments.
      - KM: C Deployment to different environments is interesting. Deploying to different environments (as many as you like) is part of the overall CI/CD process in Jenkins X.
      - TM: There are many differnt camps. Great to discuss further.
      - TM: Will take on role of discussing futher with members to find agreement on these terms.
      - TM is now Executive Director of CDF. Woohoo! 🎉
      - TM: Starting off with these definitions key and happy to push things forward.
      - EB & AG: Discuss additions on defining Events in CI/CD 
  - Updates by EB & AG from Events in CI/CD workstream, Workstream Reps
      - [Workstream docs](https://github.com/cdfoundation/sig-interoperability/tree/master/workstreams/events_in_cicd)
      - EB: Have had a few initial meetings, and current focus is to develop event vocabulary in CI/CD context.
      - AG: Will be adding to whitepaper and will summarise findings.
  - CI/CD at GoSpotCheck, Dave Sudia, GoSpotCheck
  - RA: Great talk by Dave. The challenges GoSpotCheck are facing and working through are exactly similar to what ebay is also experiencing.
  - TM: Great talk. Question on the shift to K8s, what was the process? Small steps? Process complete?
  - Dave S: IProcess complete except for a few minor long tail microservices.
  - KM: Interesting that the need for Support to be at the table, especially as with Canary Deployments a section of customers may well be experiencing breaks, etc. Would feature previews be helpful: https://github.com/jenkins-x/enhancements/issues/41
  - Dave S: Will comment on issue, happy to discuss further with team as well. 
  - RA: Properly using microservices requires a good deal of maturity in the team and import to do right or will be in a world of pain. (General agreement)
  - KM: one of the things we do with Jenkins X (and have suggested to other teams/companies) is using version streams. (Dave: would be open to follow up discussion on version streams)
  - TM: What cloud are you on? Multi-cloud? Or interest / concerns around multi-cloud.
  - Dave S: 90% GCP. Some buckets, data pipelines on AWS (that is mostly legacy set up and may migrate data pipelines to GCP). Multi-cloud or vendor lock-in is not so much of a concern. Not big enough to really feel that need. In terms of cloud providers, keeping a lid on costs is key priority.
  - \<addme\>

#### Action Items
  - Fatih to open a new issue and ask CDF to include Zoom meeting link on it: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/213)
  - Tracy M: Further discussions with individuals and teams on CI/CD definitions.
  - Folks can reach out to Tracy to discuss these terms.
  - Tracy: Will use powers to update meeting invite with zoom link. 🙏
  
#### Meeting Recording
  - https://www.youtube.com/watch?v=0dbZwahf0qc&list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG&index=2&t=0s

### August 20, 2020

#### Participants
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Dave Sudia (GoSpotCheck)
  - Ravi Lachhman (Harness)
  - Emil Bäckmark (Ericsson)
  - Mattias Linnér (Ericsson)
  - Jerop Kipruto (Google)
  - Christie Wilson (Google)
  - Cameron Motevasselani (Armory)
  - Eric Sorenson (Puppet)
  - Jeremy Stanley (OSF/Zuul)
  - Kara de la Marck (CloudBees)

#### Agenda and Notes
  - Action Item Review, All
  - Reusable Libraries, All
      - KM: Had a preliminary meeting to discuss Helm 3 Chart. There are people who are onboard with the idea.
      - KM: https://github.com/tektoncd/pipeline/issues/1542
  - CI/CD Interoperability Whitepaper, All
      - Outline: https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit
      - Definitions: Continuous Integration, Continuous Delivery, Continuous Deployment
      - What does interoperability mean in CI/CD context
      - Trends: Reusable Libraries, Events in CI/CD
      - Potential Case Studies: Dave Sudia/GoSpotCheck, Emil Backmark/Ericsson, Jeremy Stanley/Zuul, Kara de la Marck/Jenkins X, Cameron Motevasselani/Spinnaker
      - The topic will be revisited during upcoming SIG meetings regulary. Towards the end of September, we could attempt to set a target date to publish the paper, granted that we covered the topics sufficiently.
  - TektonCD at eBay, Ramin Akhbari (eBay)

#### Action Items
  - Fatih to open a new issue and ask CDF to include Zoom meeting link on it: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/213)
  - ~~Tracy to arrange a meeting to discuss way forward with hosting Tekton Helm 3 Chart in CDF~~
  - ~~Fatih to send mail on whitepaper to maillist~~
  - ~~Fatih to talk to Jacque to update the invitation with HackMD link: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/201).~~
  

#### Meeting Recording
  - https://www.youtube.com/watch?v=tdKnEEZGZ0U

### August 6, 2020

#### Participants
  - Andrew Bayer (CloudBees)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Andreas Grimmer (Dynatrace)
  - Dave Sudia (GoSpotCheck)
  - Kara de la Marck (CloudBees)
  - Gareth Evans (CloudBees)
  - James Rawlings (CloudBees)
  - Ramin Akhbari (eBay)
  - Christie Wilson (Google)
  - Tracy Miranda (CloudBees)

#### Agenda and Notes
  - Action Item Review, All
  - Publicizing the work we are doing, All
      - Should we start working on publishing something like a whitepaper to talk about the challenges, trends, progress and call-for-action?
      - James and Kara: Can help from Project/Jenkins X perspective.
      - David and Ramin: Can help from end-user point of view.
      - Tracy to help with CDF.
      - Link to outline: https://docs.google.com/document/d/1Bgr6EHhW4wUTphU8xyMg87qzSee43PEA_gGdMnPHq9Q/edit
      - This could be brought up to CDF Ambassador call for contributions.
  - Reusable Libraries, All
      - Should we have a workstream to drive & coordinate this work and work with setting things up?
      - TM: Re: Tekton Helm 3 Chart in CDF - I can setup a session to bring few people together to figure out what it means. 
      - TM: 13th August 2020 - working session for Tekton Helm 3 chart repo in CDF (same time as interop sig meeting)
  - [Lighthouse](https://github.com/jenkins-x/lighthouse) Presentation, Andrew Bayer, CloudBees

#### Action Items
  - Tracy to arrange a meeting to discuss way forward with hosting Tekton Helm 3 Chart in CDF
  - Fatih to send mail on whitepaper to maillist
  - **In progress**: Fatih to talk to Jacque to update the invitation with HackMD link: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/201).

#### Meeting Recording
  - https://www.youtube.com/watch?v=HyyHI065S_o

### July 23, 2020

#### Participants
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci (Ericsson Software Technology)
  - James Rawlings (Jenkins X / CloudBees)
  - Kara de la Marck (CloudBees)
  - David Sudia (GoSpotCheck)
  - Tracy Miranda (CloudBees)
  - Cameron Motevasselani (Armory / Spinnaker)
  - Ryan Pei (Armory)
  - Thanh Ha (Lumina Networks)

#### Agenda and Notes
  - Action Item Review, All
  - Approve/discuss [moving Roadmap to repo](https://github.com/cdfoundation/sig-interoperability/pull/40).
      - Discussed, general approval. PR merged; Roadmap added to sig-interoperability repo.
  - Tekton Pipelines Helm Chart: https://github.com/tektoncd/pipeline/issues/1542
      - JR: move Tekton Helm chart into repo under CDF
      - FD: propose to TOC having library
      - TM: Will sync with Tekton community and discuss the way forward
      - DS: as an end user having a utility etc hosted by a foundation such as CDF is highly reassuring.
      - FD: CDF repos will be good for visibility for cross-project assets like the Helm charts
  - go-scm
      - KM: Reached out to folks to start the discussion. If the SIG thinks this is the way, we could contact Tekton folks.
  - [Spinnaker](https://spinnaker.io/) Presentation, Cameron Motevasselani, Armory
      - RA: question on Spinnaker, what was the result of investigation into using Tekton as the engine within Spinnaker rather than Orca
      - CM: We are not doing that at the moment, but it is something that would be interesting to do in future
  - Tekton & Jenkins POC 
      - https://www.jenkins.io/events/ Friday 24th, 7am Eastern

#### Action Items
  - **In progress**: Fatih to talk to Jacque to update the invitation with HackMD link: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/201).
  - ~~Marky to check with Jacque the possibility of storing none-meeting recordings on Youtube: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/202).~~

#### Meeting Recording
  - https://www.youtube.com/watch?v=vBJJoajJAVU

### July 9, 2020

#### Participants
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Emil Bäckmark (Ericsson)
  - James Rawlings (CloudBees)
  - Max Körbächer (Storm Reply)
  - Kara de la Marck (CloudBees)
  - Thanh Ha (Lumina Networks)
  - Marky Jackson (OpsMX)
  - Jeremy Stanley (Zuul community)
  - Oleg Nenashev (CloudBees)
  - Mark Waite (CloudBees)
  - Tracy Miranda (CloudBees)

#### Agenda and Notes
  - Action Item Review, All
  - [SIG Roadmap](https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit#heading=h.eqpoxxy8gmzz) in the repo, All
    - FD: A [pull request](https://github.com/cdfoundation/sig-interoperability/pull/40) is opened, moving the roadmap from Google Docs to SIG repository on GitHub.
    - FD: Few updates have been made to the roadmap while moving it to the repo such as adding the presentations that were made to the SIG.
    - FD: In addition to the updates, the new work we started doing such as identifying Focus Areas and creating workstreams is also included in the document.
    - FD: Contributors are also listed on the document.
    - FD: PR will be kept open few more days to give people chance to review it and provide comments.
    - FD: Once we finalize the work with the roadmap, we could ask CDF to help us to make this work visible via a blog post/article.
    - MJ: I can help with that.
  - SIG Governance, [workstream setup](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/workstream-governance.md), Kara, All
    - KM: The governance document for the workstreams is [now available in the repo](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/workstream-governance.md).
    - KM: People who are interested in working on a specific topic are encouraged to create a PR and socialize the idea by presenting it during upcoming SIG meetings to collaborate with others.
    - MK: WG Robots could be a workstream.
  - [Jenkinsfile Runner](https://github.com/jenkinsci/jenkinsfile-runner) Presentation, Oleg Nenashev, CloudBees

#### Action Items
  - ~~Fatih to move Roadmap to GitHub via a PR: https://github.com/cdfoundation/sig-interoperability/pull/40~~
  - ~~Tracy to take SIG Roadmap document into read-only/comment-only mode~~
  - ~~Kara to update workstream governance with the process for creation of new workstreams: https://github.com/cdfoundation/sig-interoperability/pull/39~~
  - **In progress**: Fatih to talk to Jacque to update the invitation with HackMD link: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/201).
  - **In progress**: Marky to check with Jacque the possibility of storing none-meeting recordings on Youtube: [Issue created in CDF backlog](https://github.com/cdfoundation/foundation/issues/202).

#### Meeting Recording
  - https://www.youtube.com/watch?v=vnuEV8pHKD8

### June 25, 2020

#### Participants
  - Kara de la Marck
  - Marky Jackson (OpsMX)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Ravi Lachhman (Harness)
  - James Rawlings (CloudBees / Jenkins X)
  - Emil Bäckmark (Ericsson)
  - Andreas Grimmer (Dynatrace)
  - Gareth Evans (Jenkins X)
  - Venkata Shreyas Kabekkodu (Fidelity)

#### Agenda and Notes
  - Action Item Review, All
  - Way forward with [SIG Roadmap](https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit#heading=h.eqpoxxy8gmzz), All
    - EB: Added Argo Rollouts under Knowledge Transfer in CI/CD tools in the roadmap.
    - EB: Added example CI and DevOps/Continuous Feedback activities into the roadmap and it is open for feedback.
    - FD: The roadmap has been around and it may make senseto move the document to GitHub into SIG repository so any further updates and conversations on the roadmap could happen in the repository.
    - No objection has been rasied by the participants of the meeting .
  - SIG Governance, [workstream setup](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/workstream-governance.md), Kara, All
    - KM: First version of the workstream setup has been made available in the repo.
    - RL: We self-organized and mimicking the SIG meeting setup.
    - FD: The idea with the workstream setup is to help people to work on specific topics without hinderance or loss of focus due to broader list of topics discussed within the SIG.
    - RL: We started very recently and we don't have much to say at the moment.
    - EB: The workstream meeting notes are kept within [SIG repository](https://github.com/cdfoundation/sig-interoperability/tree/master/workstreams/events_in_cicd).
    - KM: Sharing the findings, learnings, outcomes from the workstream with the broader SIG would be very valuable. Cadence is up to the workstreams.
    - EB: The initial thought within the workstream was that we were aligned in the thinking of some fundamental aspects like "what is event".
    - EB: We found out that there are differences in thinking so we are working on that.
    - AG: The first meeting was about collecting material and we are at the starting point.
    - KM: How people can come up with new workstream ideas?
    - FD: Anyone should be able to propose new workstreams by simply creating an issue in the repo and adding a topic to the SIG meeting so the workstream idea can be publicized/socialized with the broader community.
    - KM: I have an idea about a workstream on Tekton Catalog.
    - JR: We want to have good interop story and good citizens while sharing our learnings.
  - Topics for CDF Project Collaboration Working Summit, Fatih, All
    - Potential topics are: Reusable Libraries (go-scm, etc), Events in CI/CD (Tekton, Keptn, Eiffel)
    - Cross project demos? 
    - MJ: Might be good to have discussions on some of the project interoperability work that is being done.
    - Examples include: Jenkins + Spinnaker, Jenkins X and Tekton, etc
    - Show work that is being done and use this work as examples of interoperability and sharing practices.
    - JR: Great if we could develop specifications or open standards 
    - FD: Question on date, as many could be on summer holidays.
    - MJ: That is being considered, more info coming on mail list
    - MJ: the format will be similar to unconference -- individuals can propose topics in slack in advance (with voting). The agenda for the day will be based on the advance voting.
  - Upcoming Presentations, Kara
    - [Schedule is updated](https://docs.google.com/document/d/1Owg_I52WEXzqF8g_lX6OTdwbHkH4Z2-7TBA7eCSVMqY/edit)
    - KM: Lighthouse and Spinnaker presentations are scheduled for July 9 and July 23.
    - EB: Argo Events and Argo Workflow are the other Argo projects which may be interesting to have presentations on.
    - EB: Argo terms could be included in the vocabulary 

#### Action Items
  - Fatih to move Roadmap to GitHub via a PR
  - Tracy to take SIG Roadmap document into read-only/comment-only mode
  - Kara to update workstream governance with the process for creation of new workstreams
  - **In progress**: Fatih to talk to Dan Lopez to update the invitation with HackMD link: [Issue created in CDF Foundation backlog](https://github.com/cdfoundation/foundation/issues/201).
  - **In progress**: Fatih/Kara to check with Dan Lopez and Jacque the possibility of storing none-meeting recordings on Youtube: [Issue created in CDF Foundation backlog](https://github.com/cdfoundation/foundation/issues/202).
  - ~~Everyone to review the roadmap and provide feedback as to whether it is ready to be added to GitHub.~~
  - ~~Kara to start the document on SIG governance, esp workstreams.~~ 
  - Chun to reach out to Brandon from Drone community for go-scm library
  - ~~Tracy and Kara to invite Andrew Bayer, Christie Wilson, and James Rawlings to discuss go-scm~~
  - ~~Tracy to reach out to Spinnaker folks - Kara invited representative from Spinnaker community~~

#### Meeting Recording
  - https://www.youtube.com/watch?v=hjhttOywNIE

### June 11, 2020

#### Participants
  - Andreas Grimmer (Dynatrace)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Max Körbächer (Storm Reply)
  - Kara de la Marck (CloudBees)
  - Christie Wilson (Google) (first half only 🙏)
  - Emil Bäckmark (Ericsson)
  - Alejandro Andreu (N26)
  - Thanh Ha (Lumina Networks)
  - Danny Thomson (Intuit)
  - Vaidik Kapoor (Grofers)
  - Ramin Akhbari (eBay)

#### Agenda and Notes
  - Action Item Review, All
  - Way forward with [SIG Roadmap](https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit#heading=h.eqpoxxy8gmzz), All
      - FD: Should we move the current version to the repo, review, and approve it as the first version?
      - FD: The topic will be discussed again coming weeks
  - Way of working with focus areas (workstream, eg.), All
      - FD: Could be taken out of Roadmap and documented in the repo as part of SIG Governance
      - KM: Can start the document.
  - Reusable Libraries, Tracy Miranda, Chun-Hung Hsiao
      - CW: go-scm is a go library lets you interact with SCM in an easier way. Tekton used go-scm to interact with SCM.
      - CW: Jenkins X also uses it but on a fork so there are 2 versions of it (Tekton uses this fork).
      - CW: Reached out to Drone folks about it but not much feedback. (https://discourse.drone.io/t/go-scm-jenkins-x-tekton-and-cdf/6698)
      - EB: Is there shared/common vocabulary defined in this library?
      - CW: Definitely there is and the terminology can be extracted from it.
          - I think this is the interface that go-scm defines: https://github.com/jenkins-x/go-scm/blob/ece1d8bc9314201c3a29d9b042e209e40bdcec89/scm/client.go#L83-L117 (go-scm could definitely use some more docs - have to point at the code to show you the interface)
      - KM: Andrew Bayer can do a presentation on it, from Jenkins X point of view, and on [Lighthouse](https://github.com/jenkins-x/lighthouse). 
  - Events in CI/CD, Emil Bäckmark, Andreas Grimmer, Ravi Lachhman, Ramin Akhbari
      - EB: The workstream was initiated and the first meeting happened on June 8. Emil, Andreas, Ramin, Ravi, and Emelie started talking about what the workstream is about.
      - EB: The proposed name "Event Driven CI/CD" feels a bit restrictive so we renamed it to "Events in CI/CD" in order not to restrict ourselves at this phase.
      - EB: Discussed the terminology such as "what is event" and so on
      - EB: Minutes are added to sig-interoperability repository and available on [HackMD](https://hackmd.io/QijjoIAiSeCNhaLpXhr05w).
      - RA: The meeting recordings could be put on non-personal channel. 
      - EB: Not sure how valuable it is to put it on Youtube.
      - AG: Agreed with question of value of having the recordings on YouTube
      - CW: Good to have recordings for those who can't attend. Could use a Google Drive.
      - Other possibility is to have second YT channel.
  - [WG/SIG CI Robots](https://github.com/cdfoundation/toc/issues/77) proposal to be discussed, Max Körbächer
      - MK: Use of robots in pipelines quite common, eg Robot Framework, CI/CD testing framework. 
      - MK: These robots are often focused on interfacing with humans (ChatOps)
      - MK: Would be good to explore how these tools can be interchanged
      - AG: Would be great to have this initiative join SIG "Events in CI/CD" workstream. Invitation to join the SIG
      - MK: That would be good.
      - FD: As the proposal to create the WG/SIG CI Robots was made to the TOC, this invitation needs to be recorded on that proposal. 
  - Presentation on [Argo Rollouts](https://argoproj.github.io/argo-rollouts/) by Danny Thomson from the Argo Team
      - How does this differ from native Kubernetes capabilities?
      - DT: Deployment object provides ability to do rolling updates, but not blue/green deployments, canary deployments, etc
      - AG: GitOps friendly? Persist state of Argo Rollout in GH? 
      - DT: what is stored in git repo is analysis template. That is blueprint stored in git while analysis runs as an instantiation of that template.
      - AG: duration for rollouts can be limited by external factors such as time of day, number of users at that tim, etc.
      - DT: in template can set benchmarks that need to be met in the analysis prior to promotions
      - AA: motivation for creating Argo Rollouts (given Flagger).
      - DT: 1) work started soon after Flagger released, so wasn't on their map yet 2) Argo Rollouts initially focused on blue/green use case. 3) differnces in approaches
 

#### Action Items
  - Fatih to talk to Dan Lopez to update the invitation with HackMD link
  - Everyone to review the roadmap and provide feedback as to whether it is ready to be added to GitHub.
  - Kara to start the document on SIG governance, esp workstreams. 
  - Fatih/Kara to check with Dan Lopez and Jacque the possibility of storing none-meeting recordings on Youtube
  - Chun to reach out to Brandon from Drone community for go-scm library
  - Tracy and Kara to invite Andy Bayer, Christie Wilson, and James Rawlings to discuss go-scm
  - ~~Andreas to reach out to Argo folks~~
  - Tracy to reach out to Spinnaker folks

#### Meeting Recording
  - https://www.youtube.com/watch?v=ZMfoGg2BM2E

### May 28, 2020

#### Participants
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Ravi Lachhman (Harness)
  - Emil Bäckmark (Ericsson)
  - Kara de la Marck (CloudBees)
  - Chun-Hung Hsiao (D2iQ)
  - Tracy Miranda (CloudBees)
  - Jerop Kipruto (Google)
  - Andreas Grimmer (Dynatrace)
  - Jeremy Stanley (OpenDev)
  - Jacqueline Salinas (LF/CDF)

#### Agenda and Notes
  - Action Item Review, All
  - SIG Co-chair, All
      - FD: [Nomination period started](https://lists.cd.foundation/g/sig-interoperability/message/38) on 2020-05-19 and ended on 2020-05-28.
      - FD: Kara de la Marck was [nominated by](https://lists.cd.foundation/g/sig-interoperability/message/40) Tracy Miranda as SIG co-chair and she [accepted](https://lists.cd.foundation/g/sig-interoperability/message/43) the nomination.
      - FD: Kara is the new co-chair for the SIG.
      - Kara introduces herself.
  - New Member Introduction
      - Chun from D2IQ
      - Jerop from Google from Tekton Community
      - Ravi from Harness
  - [Proposed focus areas in SIG Roadmap](https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit#heading=h.bb9yec6zfdei), All
      - FD: The areas proposed on the document has been discussed.
      - FD: The 2 of them, reusable libraries and event driven CI/CD, got interest from the meeting participants.
      - FD: The people who shown interest to these areas could perhaps start talking about how to move this forward and SIG could then take another discussion on the proposed way forward.
      - FD: Please see the [meeting recording](https://www.youtube.com/watch?v=Z-Ihwminsc0) for the discussion.
  - Interoperability Summit
      - TM: To bring representatives from various projects to discuss topics. Reach out to Dan Lorenc for more details.
  - Topics for upcoming meetings
      - TM: Do we need more outreach?
      - Spinnaker?
      - Harness presentation/demo from Ravi
      - Argo presentation/demo
      - Tekton based platforms?
      - GitHub?
  - Interoperability Podcast
      - JS: Published - 101 downloads - [Podcast](https://cdeliveryfdn.buzzsprout.com/1008697/3778943-cdf-sig-interoperability-chair-cloudbees-puppet-discuss-interoperability)
      - JS: Followup podcasts - anyone interested to take part in the podcast, please reach out to Jacque

#### Action Items
  - Chun to reach out to Brandon from Drone community for go-scm library
  - Tracy to invite Andy Bayer, Christie Wilson, and James Rawlings to discuss go-scm
  - Andreas to reach out to Argo folks
  - Tracy to reach out to Spinnaker folks

#### Meeting Recording
  - https://www.youtube.com/watch?v=Z-Ihwminsc0

### May 14, 2020

#### Participants
  - Fatih Degirmenci, Ericsson Software Technology
  - Emelie Pettersson, Ericsson
  - Kara de la Marck, CloudBees
  - James Rawlings, CloudBees
  - Christie Wilson, Google
  - Vincent Demeester, Red Hat
  - Tracy Miranda, CloudBees
  - Eric Sorenson, Puppet
  - Ramin Akhbari (eBay)
  - Manuel Stein
  - Jack Morgan
  - Jeremy Stanley, OpenDev

#### Agenda and Notes
  - Action Item Review, All
  - SIG Co-chair, All
      - CW: I was excited to contribute as co-chair the SIG but I don't think I will have time to do that.
      - Agree: Nomination period will start on 2020-05-15 on the SIG Maillist
  - [SIG Update to TOC](https://docs.google.com/presentation/d/169XI0xHzltPJfGI4ZBSoZ1-y0DLabe8uKueDbsW9f8E/edit?usp=sharing), All
      - TM: The update was well received by the TOC.
  - SIG Outreach
      - TM: [CDF Interoperability Newsletter](https://cd.foundation/stay-connected/newsletter-archive/) went out. 4 articles, including the shared vocabulary article was published.  
      - TM: Highlighted at CDF member meeting.
      - TM: The theme for the June issue of the newsletter is MLOps.
  - [SIG Roadmap](https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit#heading=h.8ve85us1mswx), All
      - FD: A new chapter, Focus Areas, has been added, listing few uses cases based on the discussions taken during the past meeetings and from project & end user presentations.
      - FD: In addition to use cases, some areas to focus also proposed together with possible way to work on them by creating a workstream per area.
      - FD: A discussion will be kicked off on maillist to see if the areas proposed on the roadmap make sense and identify what other areas we could focus on.
      - RA: One of the challenges we see is the quality gates in the pipelines.
  - Presentation on Tekton Catalog + Tekton Hub, Christie Wilson + Vincent Demeester 👼
  - SIG Meeting Recordings
      - FD: All the meeting recordings (except the very first one) is available on CDF Youtube Channel.
      - FD: See [SIG Interoperability Playlist](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG) for the list of recordings.

#### Action Items
  - Kick of co-chair nominations on SIG Maillist, Fatih Degirmenci
  - Start the discussion around SIG Roadmap on Maillist

#### Meeting Recording
  - https://www.youtube.com/watch?v=pgEqYfT4whg

### April 30, 2020

#### Participants
  - Emil Bäckmark, Ericsson
  - Emelie Pettersson, Ericsson
  - Max Körbächer, Storm Reply
  - Stefan Prodan, Weaveworks
  - James Rawlings, CloudBees
  - Tracy Miranda, CloudBees
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci, Ericsson Software Technology
  - Kara de la Marck, CloudBees
  - Jack Morgan
  - Ignacio Pascual, Ericsson


#### Agenda and Notes
  - Action Item Review, All
      - FD: No action item.
  - [CDF Newsletter](https://github.com/cdfoundation/newsletter) May Issue, Tracy Miranda
      - TM: CDF Newsletter is scheduled to go out soon - today or tomorrow
      - TM: Thanks to everyone who submitted articles to the newsletter
      - TM: Please subscribe to the newsletter if you haven't done it yet and share it with your contacts
      - TM: Podcast will be published coming weeks on the topic of Interoperability.
      - TM: [Sign up for newsletter](https://cd.foundation/stay-connected/)
  - [SIG Update to TOC](https://docs.google.com/presentation/d/169XI0xHzltPJfGI4ZBSoZ1-y0DLabe8uKueDbsW9f8E/edit?usp=sharing), All
      - FD: The update to the CDF TOC will be given during the meeting on May 5th which starts at 16:00UtC. The agenda/logistics are available [here](https://docs.google.com/document/d/1uBHar55fTInWF9Li4t0lyG3tTC8BRLU0FfBfsgk_Jrs/edit?ts=5c9580be#heading=h.9z0srzj4rtji).
  - Discussion on proposed [SIG/WG CI Robots](https://github.com/cdfoundation/toc/issues/77), Max Korbi, All
      - MK: Noticed some challenges when integrating various tools/projects together.
      - MK: Everyhing that happens before CI/CD starts but on the technical level there is too much to be visible to everyone. Some auidences may not be familiar with the technical details of CI/CD and it is important to make this visible to thhose people as well.
      - MK: Three tools are mentioned - [PRobot](https://github.com/probot/probot), [Robot Framework](https://robotframework.org/) even though it is a test framework, and GitHub Bot which is an alternative, being a kind of communication interface between the pipelines and users.
      - JR: Jenkins X has automation around approving PRs, etc. using Lighthouse. When one repo changes, it is necessary to keep things in sync especially towards downstream repos.
      - MK: It is really about bridging the gap between human and the technical part of the deployment.
      - JR: ChatOps. Having ability to control and being able to extend in order to add custom controls. Related to developer experience, helping them due to having consistent way to interact with the pipelines. This is more and more important in microservices world.
      - TM: It points the need for clarity for the users.
      - RA: What is the proposal? Is it to create a standard interface for all the existing and future tools to adhere to?
      - MK: It could be one of the outcomes and there is not much available in the market. It is not utilized well and there is still quite big gap.
      - MK: SIG may be big to start with so it could be a WG to identify what we are going to work with. We will identify if this WG has any value or not during the process.
      - RA: Trying to understand what is the gap. For example Robot framework already has a protocol and interfaces of doing things, and also have libraries so what the work would be for SIG/WG to do.
      - MK: This could be one of the outcome of the work proposed SIG/WG does. It would be interesting to understand to see how the integration between Robot & Prow with Github and so on. It may be difficult to adapt these to your own tools and pipelines. It's not yet a field with many options/tools around so we are at the phase to identify it.
      - TM: One way to approach this is to break tasks down. Everybody understtands one set of tools but not all and we can identify what tool is doing what and how these tools could operate and so on. Will look at the roadmap to see where this could be put under.
      - AP to all: Look at the roadmap to see if this fits under Next section in [Roadmap](https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit#heading=h.8ve85us1mswx)
  - [Flagger](https://flagger.app/) Presentation, Stefan Prodan, Weave Works
      - FD: Slides will be available in [CDF Presentations repository sig-interoperability folder](https://github.com/cdfoundation/presentations/tree/master/sig-interoperability).

#### Meeting Recording
  - https://www.youtube.com/watch?v=CAU7-qbNZo0

### April 16, 2020

#### Participants
  - Eric Sorenson (Puppet)
  - Fatih Degirmenci (Ericsson Software Technology)
  - Emelie Pettersson (Ericsson)
  - Andreas Grimmer (Dynatrace)
  - Tracy Miranda (CloudBees)
  - Ramin Akhbari (eBay)

#### Agenda and Notes
  - Action Item Review, All
  - Hackmd.io migration for meeting agenda and minutes, All
    - FD: Integration with GitHub - single source of truth
    - FD: Collaborative editing
    - TM: Used it and it seems to be straightforward.
    - Agree: Meeting minutes will be moved to HackMD.io from the meeting on 2020-04-30 and onwards
  - CDF Newsletter, All
    - TM: Newsletter will go out end of April 30
    - TM: Few article proposals have been received on Tekton, Jenkins X, SIG Vocabulary, Jenkins and Spinnaker Integration
    - TM: Newsletter is open to contributions from anyone.
    - TM: Jacqueline is looking for a panel and there may be a virtual session.
  - SIG Interoperability Roadmap, All
    - TM: The document outlines the charter
    - AG: End users could be software engineers, managers and so on. What kind of tools they use and the types of requirements the different audiences have.
    - AG: In order to identify the interfaces, it is important to understand common tasks first - deployment, testing, release, and so on. This could help us to identify the interfaces.
    - Discussion on how to highlight, share, and reach to a shared vocabulary in CI/CD domain. Reaching out to projects, experts, bringing this to CDF TOC’s attention.

#### Meeting Recording
  - https://www.youtube.com/watch?v=7LNYbQBrtvY
  
### April 2, 2020

#### Participants
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci, Ericsson Software Technology
  - Andreas Grimmer (Dynatrace)
  - James Rawlings (CloudBees)
  - Eric Sorenson (Puppet)
  - Emil Bäckmark, Ericsson
  - Tracy Miranda, CloudBees
  - Jacqueline Salinas, LF/CDF
  - Minoru Nitta
  - Jack Morgan
  - Emelie Pettersson, Ericsson

#### Agenda and Notes
 - Action Item Review, All
    - FD - reached out to Spinnaker/Armory to get representation, hasn't gotten response
    - TM - will ask Rosalind next week. Could do shout-out at next TOC to see if there are additional folks who would like to join.
    - AG - Sumit Nagal from Argo/Intuit
    - All - open PR on vocabulary addition from Keptn, review and merge
    - SIG Interoperability Roadmap, All
    - TM: Folks started contributing. The doc started to take shape. Everyone is welcomed to provide feedback, put comments, new suggestions. The document can later be moved to GitHub repo.
    - ES: Is there a target date to finish the initial work?
    - TM: Would be good to get the first working version ready during next month.
    - CDF Newsletter: Interoperability Theme for April, Tracy M
    - TM: A lot of things are happening in CDF Outreach Committee and one of the ideas is to drive specific topics. April topic is Interoperability. In terms of the newsletter is to curate articles on interoperability and articles from Eric & Andreas are under the radar. Articles on how Tekton works with Jenkins X, how Spinnaker works with Jenkins, etc. If anyone has interest in writing an article for the newsletter, reach out to Tracy. They will be reviewed by Outreach Committee.
    - TM: Coming months have topics on MLOps, Security.
    - Jaque Salinas: about 866 people currently subscribed.
    - ES: The article was about on the latest changes in Tekton, triggers and so on.
    - Andreas article here: https://medium.com/keptn/scaling-continuous-delivery-and-runbook-automation-via-tool-interoperability-interfaces-5ded97eceb3b
    - Eric part1: https://medium.com/relay-sh/whats-going-on-with-tekton-part-1-9c3e006d39fc , part 2: https://medium.com/relay-sh/whats-going-on-with-tekton-part-2-ab39176c9c45
  - Jenkins X Presentation, James Rawlings, CloudBees (See video)

#### Meeting Recording
  - https://www.youtube.com/watch?v=8S98BUZQKRM

### March 19, 2020

- **Participants**
  - Ramin Akhbari (eBay)
  - Fatih Degirmenci, Ericsson Software Technology
  - Andreas Grimmer, Dynatrace
  - Emelie Pettersson, Ericsson
  - Jeremy Stanley, OpenDev
  - Eric Sorenson, Puppet
  - Terry Cox, Bootstrap
  - Andrew Bayer, CloudBees
  - Tracy Miranda, CloudBees
  - Emil Bäckmark, Ericsson (last half hour only)

- **Agenda and Notes**
  - SIG Interoperability Roadmap, Tracy Miranda, CloudBees
    - TM: WIP/Draft Roadmap: https://docs.google.com/document/d/1QSzcV-rl3XwkNh4_5a_0YCugF5gprtBR-xRlzuEJ-NA/edit?usp=sharing
    - TM: Best practices for the roadmap for groups like this is not to focus on specific dates but use time horizon.
    - TM: Charter for the SIG is summarized in the document.
    - TM: Some of the outcomes are knowledge transfer of CI/CD tools, the terminology, end user requirements and keeping them in mind, shared reference terminology to enable people communicate with each other, interoperable tools, standardized frameworks, promoting best practices
    - TM: Time horizons in the document are current, near term, and future.
    - TM: Some of the topics for each of these are listed there as an input.
    - RA: Are Spinnaker and Codefresh represented in the SIG since they are gathering different use cases from the industry and can provide a lot of input to the SIG.
    - FD: Unfortunately not.
    - TM: Feel free to contribute!
  - Next steps with the vocabulary, All
    - FD: Should we try to come up with something like “shared vocabulary” as it was intended originally?
    - TM: CDF Outreach Committee started working on different posts on various areas and this could be something to get the word out.
  - Do we want to have any kind of facilitator rotation? Christie Wilson, Google
    - ES: I can help out with this.
  - Zuul Presentation, Jeremy Stanley, OpenDev
    - JS: Slides: http://fungi.yuggoth.org/presentations/2020-cdf/slides.html

- **Action Items**
  - Reach out to Spinnaker (Netflix/Armory) and Codefresh and invite them, Fatih Degirmenci

#### Meeting Recording
  - https://www.youtube.com/watch?v=TLgcjYe_joM

### March 5, 2020

- **Participants**
  - Andrew Bayer, CloudBees
  - James Rawlings CloudBees
  - Emil Bäckmark, Ericsson
  - Fatih Degirmenci, Ericsson Software Technology
  - Ethan Jones, CloudBees
  - Andreas Grimmer, Dynatrace
  - Ramin Akhbari (eBay)
  - Terry Cox, Bootstrap
  - Jeremy Hartley, CloudBees
  - Christie Wilson, Google
  - David Blaisonneau, Orange
  - Minoru Nitta
  - Tracy Miranda, CloudBees
  - Jeremy Stanley, OpenDev

- **Agenda and Notes**
  - Action Item Review, All
  - SIG Interoperability Roadmap, Tracy Miranda, CloudBees
    - FD: Postponed to the next meeting.
  - Google Summer of Code, All
    - FD: CDF is taking part in [Google Summer of Code](https://summerofcode.withgoogle.com/organizations/5550056498790400/)
      If anyone has a project idea, please reach out to Dan Lopez and Jacqueline Salinas to find out how you can get your project part of GSoC.
  - [Keptn](https://keptn.sh/), Andreas Grimmer, Dynatrace
    - FD: Meeting is recorded and it will be published on CDF Youtube Channel.
    - FD: Presentation will be stored in [cdf presentations repository sig-interoperability folder](https://github.com/cdfoundation/presentations/tree/master/sig-interoperability)
  - GitLab Pipelines, David Blaisonneau, Orange
    - FD: Meeting is recorded and it will be published on CDF Youtube Channel.
    - FD: Presentation will be stored in [cdf presentations repository sig-interoperability folder](https://github.com/cdfoundation/presentations/tree/master/sig-interoperability)

- **Action Items**
  - Store Keptn presentation in cdf/presentations repository sig-interoperability folder, Andreas Grimmer, Dynatrace
  - DONE: Store Orange Gitlab Pipelines presentation in cdf/presentations repository sig-interoperability folder, David Blaisonneau, Orange

#### Meeting Recording
  - https://www.youtube.com/watch?v=cREQjs5hDLY

### February 20, 2020

- **Participants**
  - Jason Yavorska, GitLab
  - Emelie Pettersson, Ericsson
  - Ramin Akhbari, eBay
  - Fatih Degirmenci, Ericsson Software Technology
  - Kara de la Marck, CloudBees
  - Christie Wilson, Google
  - Tracy Miranda, CloudBees
  - Jeremy Hartley, CloudBees
  - Orit Golowinski, GitLab
  - Ignacio Pascual, Ericsson

- **Agenda and Notes**
  - SIG Interoperability Co-chairs
    - FD: Nomination period ended on February 10th and 2 people were nominated by others  - Christie Wilson and Wavell Watson.
    - FD: Christie Wilson accepted the nomination but Wavell Watson didn’t by the time the nomination ended so Christie Wilson becomes the new co-chair.
  - [Common vocabulary/terminology](https://github.com/cdfoundation/sig-interoperability/pull/14)
    - TM: We can merge the document as is and ask people to contribute it by issuing new PRs
    - TM: A blog post can be published to promote the vocabulary/terminology
  - [Starting the work on SIG Goals, Roadmap](https://github.com/cdfoundation/sig-interoperability/issues/15)
    - FD: Looking for contributors
    - CW: One way this could go is that this SIG could work on creating standards.Another idea about the SIG is to keep track of what’s happening in industry.
    - TM: Roadmap is important to identify low hanging fruits to get momentum, get more people, starting to tackle some challenges
    - CW: We could start highlighting some tools that are currently interoperate and highlighting some challenges to make sure people know why this topic is important.
    - TM: Initial categories, the way to deal with them. Rather than laying out that we will do this or that in specific time, we could focus on what we are doing now,
      what we will focus next so people can start contributing to those ideas. Will take first stab.
  - Discussion around [standardization of container-based step execution](https://docs.google.com/document/d/1geL8hMN3Qy5C7lJTb6MUCPquDzwsU022eRUr4nGdI44/edit)
    Jason Yavorska, GitLab
    - Also look at CircleCI orbs, Github Actions e.g. how do we run sth from github actions in Tekton
    - CW: [Tekton Notifications Proposal](https://docs.google.com/document/d/1ehhGngn2ulnjYX0HUxSyhQGAvcbabSa27UZs3RvZWwU/edit)
    - CW: This might take Christie a bit to figure out how to share the document but in the meantime if you join the tekton-dev@ mailing list you’ll get access right away!
    - CW: Tekton docs: https://github.com/tektoncd/pipeline/tree/master/docs#tekton-pipelines
    - CW: Tekton task docs: https://github.com/tektoncd/pipeline/blob/master/docs/tasks.md
    - FD: Please see the meeting recording for the discussion.
  - KubeCon Amsterdam
    - TM: Who is going? There will be discussions around common metadata to describe deployments.
    - FD: It might be a good idea to send mail to CDF SIG and/or TOC maillists to let people know about the discussions during KubeCon.
    - CW: CD Summit will happen as day-zero event on March 30.
    - CW: [CD Summit Schedule](https://events.linuxfoundation.org/continuous-delivery-summit/program/schedule/)
  - Tekton Presentation & Discussion, Christie Wilson, Google
    - FD: Presentation will be stored in CDF presentations repo sig-interoperability folder on GitHub and recording will be posted to CDF Youtube channel.
    - CW: https://github.com/tektoncd/community#want-to-get-involved
    - FD: Presentation is available on [this link](https://github.com/cdfoundation/presentations/tree/master/sig-interoperability).

- **Action Items**
  - Take the first stab on Roadmap, Tracy Miranda
  - Provide basic examples for GitHub Actions and CircleCI Orbs, Jason Yavorska
  - Tekton Notifications Proposal is not public, Christie Wilson
  - DONE: Upload presentation to CDF presentations repo sig-interoperability folder on GitHub, Christie Wilson
  - DONE: Schedule a presentation from Jenkins X - presentation schedule is here, Tracy Miranda, Jeremy Harley

#### Meeting Recording
  - https://www.youtube.com/watch?v=0RZikpCG-6k
  
### February 6, 2020

- **Participants**
  - Fatih Degirmenci, Ericsson Software Technology
  - Emil Bäckmark, Ericsson
  - Emelie Pettersson, Ericsson
  - Terry Cox, Bootstrap
  - Jeremy Stanley, OpenDev/Zuul
  - Ramin Akhbari, ebay
  - Christie Wilson, Google
  - Tracy Miranda, Cloudbees
  - Dan Lopez, Linux Foundation

- **Agenda and Notes**
  - Action Item Review
    - FD: All action items are closed.
  - Co-chair nomination and election
    - FD: Christie Wilson and Wavell Watson have been nominated
    - FD: Co-chair nominations open until February 10
    - DLz: We don’t have to have a charter but good to adapt one.
    - DLz: Some CNCF SIGs have their own charters. https://github.com/cncf/sig-security/blob/master/governance/charter.md
    - FD + CW: Goals: Define interoperability
    - TM: ml-ops approach is good, initial roadmap, taking time to define what areas they can tackle: divide up topics, map them up
  - CD Summit Europe 2020
    - FD: CFP closes on February 7
    - FD: Event takes place on March 30
    - CW: CFPs will be reviewed by the programming committee. Program chairs will be putting the final schedule.
      The notifications will be sent out February 17th and the program will be announced after that. Lightning talks are also possible.
    - CW: Registration is open for CD Summit.
  - Work on common vocabulary/terminology
    - FD: PR is up for [review](https://github.com/cdfoundation/sig-interoperability/pull/14)
  - Presentation Template
    - DLz: CDF has a presentation template for the community to use.
    - DLz: https://github.com/cdfoundation/presentations/tree/master/templates
  - Eiffel Presentation and Discussion, Emil Bäckmark, Ericsson
    - FD: Eiffel presentation by Emil to SIG.
      Recording: https://www.youtube.com/watch?v=thr8-duWvt0
      Slides: https://github.com/cdfoundation/presentations/tree/master/sig-interoperability

- **Action Items**
  - N/A

#### Meeting Recording
  - https://www.youtube.com/watch?v=thr8-duWvt0
  
### January 23, 2020

- **Participants**
  - Fatih Degirmenci, Ericsson Software Technology
  - James Rawlings, CloudBees
  - Akin Ozer, Inveon
  - Emil Bäckmark, Ericsson
  - Terry Cox, Bootstrap
  - Eric Sorenson, Puppet
  - Dan Lopez, Linux Foundation
  - Emelie Pettersson, Ericsson
  - Tracy Miranda, Cloudbees
  - Wavell Watson, Vulk Coop/CNCF CI/CNF Testbed
  - Jeremy Stanley, OpenDev/Zuul
  - Joshua Smith, Vulk Coop/CNCF

- **Agenda and Notes**
  - Recording of meetings
    - FD: Question to all: Is everyone ok to record meetings?
    - FD: Agreed: Everyone is OK! We urge people to raise concerns if they have
      any so we stop recordings.
  - Intros
    - FD: Meeting participants introduced themselves and shared their thoughts
      regarding SIG.
  - Meeting Logistics
    - FD: Survey to determine meeting frequency/time: 10 total votes.
    - FD: Meeting frequency: 1 vote for weekly, 9 votes for bi-weekly
    - FD: Meeting time: There was a tie between 15:00-16:00UTC and 17:00-18:00UTC.
      FD opted for 15:00-16:00UTC to increase the possibility of participation
      from APAC.
    - FD: Question to all: Should we stick to UTC for meeting times?
    - FD: Summer time starts in few weeks. (US@March 8th, Europe@March 29th)
      The question was if we should stick to UTC and do not change the meeting
      time based on summer time changes or not.
    - FD: Agreed: The agreement is to stick to UTC.
  - Meeting agenda/notes
    - FD: Google Docs (this document) as working copy
    - FD: Github as the final location
    - FD: Meeting agenda and notes are kept in both places to ensure everyone
      can access those.
    - TM: hackmd.io is used by some communities and could be something we can
      look into for keeping meeting agenda and notes.
  - Invitation to join to maillist and Slack channel
    - FD: Crossposting to maillists is not considered as a good practice by
      some communities and we intend to stop doing that so we urge everyone
      to join to sig-interoperability maillist in order not to miss announcements,
      discussions, meeting information.
    - FD: Please join to #sig-interoperability channel on CDF Slack.
  - SIG Governance & Process
    - FD: Proposal is to have TOC document governance for the SIGs and we adapt it.
      See [the corresponding issue](https://github.com/cdfoundation/toc/issues/70)
      in TOC repo.
    - Adapting co-chair setup
      - FD: Question to all: Should we adapt co-chair setup that seems to be a
        common practice within CDF and CNCF SIGs?
      - FD: Agreed: Everyone is in agreement to have co-chair adapted.
      - FD: 2 additional co-chairs - 1 from projects and 1 from users to have
        different views represented.
      - TM: nominates Christie Wilson as co-chair.
      - TM: let’s give people time to think
      - JoshuaS: nominates Wavell Watson as co-chair.
    - FD: will send a mail to maillist/slack to summarize the governance discussion
      and agreement on adapting co-chair.
    - FD: will send a separate mail to start co-chair nominations.
    - Election of and terms of chair(s)
      - FD: suggestion is to have 2-year term but the question will be included
      in the mail that will be sent to SIG maillist.
  - Members of sig-interoperability team/repo
    - FD: Question to all: Who should/wants to be maintainer to sig-interoperability
    repo reviewing/merging PRs?
    - FD: Agreed: We start with the people listed as members in README.md.
  - How new-members could sign-up?
    - FD: For SIGs, the practice is to let people self-declare their interest and
    list themselves in members list if they would like to.
    - ES: Suggests to try to keep things simple which everyone agrees.
  - Upcoming presentations from users and projects
    - FD: We started inviting users/project maintainers to SIG meetings to present
    the challenges they face, the ideas they have, and the solutions they employed
    in order to increase collaboration. This will give us have chance to see and
    listen different perspectives.
    - FD: This will also make the existing work going on within interoperability
    area across projects visible.
    - FD: presentation backlog/schedule is on https://docs.google.com/document/d/1Owg_I52WEXzqF8g_lX6OTdwbHkH4Z2-7TBA7eCSVMqY/edit#
    - TM: We can invite ebay, CDF projects
  - Discussion around our vision and objectives as SIG
    - FD: README file has few points. We can perhaps make our vision and objectives
    more explicit.
  - What interoperability means in CI/CD domain?
    - FD: People have different views when it comes to interoperability
    - JR: benefits of working with various communities are huge - standardization
    and so on. Having a way to come together to start talking about interoperability
    is great.
    - FD: pipeline standardization, event driven CI/CD, pipeline language
    - JR: Tekton and Jenkins X specifications. Jenkins X created a syntax familiar
    for Jenkins users which also works for Tekton. Consistent way.
    - ES: have been looking for the opportunities with regards to interoperability
    on an individual unit level.
    - ES: Standardized declarative metadata e.g. to describe deployments
    - ES: https://docs.google.com/document/d/16e1xo1C35wBEe1skxnkgm2edGaxErhDoiN-jtIZkZM8/edit#
    - EB: look for possibilities in broader take on standardization
    - FD: being agnostic to the product is something to think about
    - WW: focusing on benefits such as: how to figure out the changes happening
    elsewhere which impacts you.
    - TC: AI/ML work done is highly regulated and CI/CD process is needed.
    Standardization/unification would be beneficial.
    - JS: There are some fundamental ideas to work with. Zuul has speculative
    execution and processes and it has pipelines. Events are used for triggering
    pipelines. Standard glossary/dictionary is needed. We need a language for humans
    to communicate first before we tackle with the tools. It would be good to see
    what people are actually dealing with.

- **Action Items**
  - ~~Join to maillist and Slack channel, All~~
  - ~~Summarize governance discussion on maillist and ask for feedback, Fatih Degirmenci~~
  - ~~Start nominations for co-chair, Fatih Degirmenci~~
  - ~~Add members listed in README.md as maintainers to sig-interoperability Github repository, Fatih Degirmenci~~
  - ~~Help us get in touch with ebay and CDF projects so we can invite them for presenting to SIG, Tracy Miranda~~

#### Meeting Recording
  - N/A