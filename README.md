# CDF Interoperability SIG

## Quick links

- [CDF Interoperability SIG](#cdf-interoperability-sig)
  - [Quick links](#quick-links)
  - [Overview](#overview)
  - [Members](#members)
  - [New Members](#new-members)
  - [Governance](#governance)
    - [SIG Workstreams](#sig-workstreams)
  - [Communication](#communication)
  - [Meetings](#meetings)

## Overview

The emergence of new open technologies and methodologies such as cloud native and
microservices has resulted in tremendous advances in various industries and enabled
the rapid development and delivery of new features and services to the end-users
faster than before. Continuous Integration (CI) and Continuous Delivery (CD) are
prerequisites and enablers for organizations to use these technologies and achieve
true agility in response to these changes.

The organizations that embrace CI/CD employ various tools and technologies depending
on their needs and where they are in their CI/CD transformation. Organizations often
employ more than one tool in various stages of their CI/CD pipelines due to different
capabilities provided by the tools. This is perhaps one of the biggest benefits the
users get by using open technologies for their CI/CD needs.

However, one of the challenges users face is the lack of interoperability across the
CI/CD tools and technologies, resulting in various issues while constructing and
running pipelines such as passing metadata and artifacts between the tools or achieving
traceability from commit to deployment. Often users end up building "own glue code" to
address what is a common problem, further complicating moving from one tool to another
and adopting new technologies and methodologies.

These "glue code solutions" are generally specific to users needs and the tools rather
than being loosely coupled and agnostic to tooling and technology. Additionally these
solutions are not visible to other users and the communities, making them vulnerable to
the risks of outage in their CI/CD pipelines due to the potential changes (ie non-backward
changes to the APIs, changes in data models) that happens to the tools in respective
projects.

SIG Interoperability will focus on addressing these challenges and further work with
projects to achieve a common set of solutions.

SIG Interoperability aims to enable a dialog in the interoperability area by bringing
CI/CD users together with the open source projects in order to

* clarify what interoperability means for the CI/CD ecosystem
* promote the need to collaborate on interoperability challenges in a neutral forum
* highlight and promote the needs of the users who face challenges constructing complex
end-to-end CI/CD flows and pipelines by employing different tools and technologies
* explore synergies between, and enable collaboration across, the CI/CD projects with
regards to interoperability
* pursue solutions which are; loosely coupled, scalable, flexible, and tool and
technology agnostic
* reduce the need for users to implement in-house solutions by promoting native
interoperability between tools
* attract and assist projects that work on interoperability

## Members

* Andy Glover ([@aglover](https://github.com/aglover)), Netflix
* Christie Wilson ([@bobcatfish](https://github.com/bobcatfish)), Google
* Eric Sorenson ([@ahpook](https://github.com/ahpook)), Puppet
* Fatih Degirmenci ([@fdegir](https://github.com/fdegir)), Ericsson Software Technology
* FuQiao ([@fuqiao123](https://github.com/fuqiao123)), China Mobile
* Kara de la Marck ([@MarckK](https://github.com/MarckK)), Cloudbees
* Priyanka Sharma ([@pritianka](https://github.com/pritianka)), Gitlab
* Thanh Ha ([@zxiiro](https://github.com/zxiiro)), Lumina Networks
* Tracy Miranda ([@tracymiranda](https://github.com/tracymiranda)), Cloudbees
* Wavell Watson ([@wavell](https://github.com/wavell)), Vulk Coop
* Ravi Lachhman ([@ravilach](https://github.com/ravilach)), Harness
* Andreas Grimmer ([@agrimmer](https://github.com/agrimmer)), Dynatrace
* Chun-Hung Hsiao ([@chhsia0](https://github.com/chhsia0)), D2iQ
* Marky Jackson ([@markyjackson](https://github.com/markyjackson-taulia)), OpsMX
* James Rawlings ([@rawlingsj](https://github.com/rawlingsj)), Cloudbees
* Ramin Akhbari ([@rakhbari](https://github.com/rakhbari)), Salesforce
* Cameron Motevasselani ([@link108](https://github.com/link108)), Armory
* Dave Sudia ([@thedevelopnik](https://github.com/thedevelopnik)), GoSpotCheck
* Andrea Frittoli ([@afrittoli](https://github.com/afrittoli)), IBM
* Oliver Nocon ([@olivernocon](https://github.com/olivernocon)), SAP SE
* Emil Bäckmark ([@e-backmark-ericsson](https://github.com/e-backmark-ericsson)), Ericsson
* Vibhav Bobade ([@waveywaves](https://github.com/waveywaves)), Red Hat
* Jerop Kipruto ([@jerop](https://github.com/jerop)), Google
* Saif Ul Islam ([@rubix982](https://github.com/rubix982)), Mapillary
* Ann Marie Fred ([@amfred](https://github.com/amfred)), Red Hat
* Melissa McKay ([@mjmckay](https://github.com/mjmckay)), JFrog
* Justin Abrahms ([@justinabrahms](https://github.com/justinabrahms)), eBay
* Brett Smith ([@xbcsmith](https://github.com/xbcsmith)), SAS Institute Inc.
* Muktesh Mishra ([@mukteshkrmishra](https://github.com/mukteshkrmishra)), Adobe

## New Members

Membership to SIG Interoperability is open to public and self-declared.

New members are advised to:

* Join the [SIG](https://lists.cd.foundation/g/sig-interoperability) and
[CDF TOC](https://lists.cd.foundation/g/cdf-toc) maillists.
* Join the #sig-interoperability channel on [CDF Slack](https://join.slack.com/t/cdeliveryfdn/shared_invite/enQtODM2NDI1NDc0MzIxLTA1MDcxMzUyMGU2NWVlNmQwN2M1N2M4MWJjOWFkM2UzMDY0OWNkNjAzNzM0NzVkNjQ5M2NkMmY2MTRkMWY4MWY) and introduce yourself.
* Go through the [README.md](README.md) document.
* Regularly join the [SIG meetings](docs/meetings.md).
* Submit a PR to add yourself to the [members list](#members).
* Here are various ways to get involved:
  * Share your thoughts by joining the meetings or by posting to maillist and Slack channel.
  * Add a topic you would like to discuss to [the agenda](docs/meetings.md) of upcoming meeting.
  * Create a [new issue](https://github.com/cdfoundation/sig-interoperability/issues) to start gathering feedback and collaborating.
  * Choose an issue where [help is needed](https://github.com/cdfoundation/sig-interoperability/issues/labels/help%20wanted)
  and comment on it expressing interest.

## Governance

SIG Interoperability is a [CDF Special Interest Group](https://github.com/cdfoundation/toc/tree/master/sigs).

The process SIG Interoperability follows can be seen from [here](https://github.com/cdfoundation/toc/blob/master/GROUPS.md#sigs).

Chairs and the TOC Sponsor of the SIG are

* Melissa McKay ([@mjmckay](https://github.com/mjmckay)), JFrog - Chair
* Kara de la Marck ([@MarckK](https://github.com/MarckK)), Continuous Delivery Foundation - Chair
* Dan Lorenc ([@dlorenc](https://github.com/dlorenc)), Google - TOC Sponsor

### SIG Workstreams

SIG Interoperability welcomes contributors who take part in the SIG to form workstreams to work on specific areas of interest
in a more focused and structured way.

Workstream governance is documented [here](./docs/workstream-governance.md).

Archived workstreams are:

* [Events in CI/CD](./workstreams/archived/events_in_cicd/README.md): now the [CDF SIG Events](https://github.com/cdfoundation/sig-events/)

## Communication

SIG Interoperability communication happens via a public mailing list and everyone is
welcome to join our open discussions.

SIG Interoperability also uses Slack for additional collaboration opportunities.

* Maillist: https://lists.cd.foundation/g/sig-interoperability
* Slack Channel: #sig-interoperability on [CDF Slack](https://cdeliveryfdn.slack.com/join/shared_invite/zt-nwc0jjd0-G65oEpv5ynFfPD5oOX5Ogg#/)

## Meetings

SIG Interoperability meets first and third Thursdays at 15:00UTC. (*See your timezone [here](https://time.is/1500_in_UTC)*).

* Meeting agenda and minutes: [here](./docs/meetings.md)
* Meeting recordings: [here](https://www.youtube.com/playlist?list=PL2KXbZ9-EY9QxICOnONBFPn_cYfJ8BsaG)
* Zoom Bridge: [here](https://zoom.us/j/827082528?pwd=RlN5OUZtVVBuZGZRY0NBRnZyZ0NJQT09)
* Zoom International dial-in numbers: [here](https://zoom.us/zoomconference)
* CDF Public Calendar (UTC): [here](https://calendar.google.com/calendar/u/0/embed?src=linuxfoundation.org_mhf0kmgedn67ihni8r129avp24@group.calendar.google.com&ctz=UTC)
