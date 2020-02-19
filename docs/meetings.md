# CDF Interoperability SIG Meetings

## Quick links

- [Logistics](#logistics)
- [Agenda and Notes](#agenda-and-notes)
  - [2020-02-20 Meeting](#february-20-2020)
  - [2020-02-06 Meeting](#february-06-2020)
  - [2020-01-23 Meeting](#january-23-2020)

## Logistics

* Google Doc: https://docs.google.com/document/d/13hCBpmuAj3e0gADo1TCjsEwmz57_fw74OhQmeY1extk
* When: every even week on Thursdays at 15:00UTC (*See your timezone [here](https://time.is/1500_in_UTC)*).
* Zoom Bridge: https://zoom.us/j/827082528
* Zoom International dial-in numbers: https://zoom.us/zoomconference
* CDF Public Calendar: [here](https://calendar.google.com/calendar/embed?src=linuxfoundation.org_mhf0kmgedn67ihni8r129avp24%40group.calendar.google.com&ctz=America%2FLos_Angeles)

## Agenda and Notes

Meeting agenda and notes are kept on [Google Doc](https://docs.google.com/document/d/13hCBpmuAj3e0gADo1TCjsEwmz57_fw74OhQmeY1extk)
and synched back to this file after the meeting.

If you have trouble accessing to the document on Google, please send a PR to add
the topic you would like discussed into the agenda.

### February 20, 2020

- **Participants**
  - \<addme\>

- **Agenda and Notes**
  - SIG Interoperability Co-chairs
  - [Common vocabulary/terminology](https://github.com/cdfoundation/sig-interoperability/pull/14)
  - [Starting the work on SIG Goals, Roadmap](https://github.com/cdfoundation/sig-interoperability/issues/15)
  - Discussion around [standardization of container-based step execution](https://docs.google.com/document/d/1geL8hMN3Qy5C7lJTb6MUCPquDzwsU022eRUr4nGdI44/edit)
    Jason Yavorska, GitLab
  - Tekton Presentation & Discussion, Christie Wilson, Google
  - \<addme\>

- **Action Items**
  - \<addme\>

### February 06, 2020

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
