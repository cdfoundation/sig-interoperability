###### tags: `CDF` `SIG Interoperability`

# CDF Interoperability SIG Meetings

[![HacmKD documents](https://hackmd.io/badge.svg)](https://hackmd.io/HuufSDMaTPyb3qxkyBKg3A?edit)

## Quick links

* [Logistics](#Logistics)
* [Meeting Recordings](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG)
* [Agenda and Notes](#Agenda-and-Notes)
    * [2022-02-03 Meeting](#February-3-2022)
    * [2022-01-20 Meeting](#January-20-2022)

## Logistics

* **Meeting notes on HackMD.io**: https://hackmd.io/@cdf-sig-interoperability/ry3TTB5DL
* **When**: First and third Thursdays at 16:00UTC (*See your timezone [here](https://time.is/1600_in_UTC)*).
* **Zoom Bridge**: https://zoom.us/j/827082528?pwd=RlN5OUZtVVBuZGZRY0NBRnZyZ0NJQT09
* **Zoom International dial-in numbers**: https://zoom.us/zoomconference
* **Meeting Recordings**: [CDF Youtube Channel SIG Interoperability Playlist](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG)
* **CDF Public Calendar**: [here](https://calendar.google.com/calendar/embed?src=linuxfoundation.org_mhf0kmgedn67ihni8r129avp24%40group.calendar.google.com&ctz=America%2FLos_Angeles)
* **Past Presentations in CDF Presentations Repository**: https://github.com/cdfoundation/presentations/tree/master/sig-interoperability
* **Presentation Schedule**: https://docs.google.com/document/d/1Owg_I52WEXzqF8g_lX6OTdwbHkH4Z2-7TBA7eCSVMqY/edit
* **2021 Meeting Minutes**: https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings_2021.md
* **2020 Meeting Minutes**: https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings_2020.md

## Agenda and Notes

Meeting agenda and notes are kept on [HackMD.io](https://hackmd.io/@cdf-sig-interoperability/ry3TTB5DL) where everyone can add new topics to the agenda for upcoming meetings or take notes during the meetings. Please click edit button to edit the document.

If you are looking for 2021 minutes of meetings, please take a look at [Meetings 2021 document](https://github.com/cdfoundation/sig-interoperability/blob/master/docs/meetings_2021.md) in SIG Interoperability repository on GitHub.

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