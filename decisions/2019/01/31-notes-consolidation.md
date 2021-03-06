# 2019/01/31: Summary of Slack discussion

There are ideas, proposals, decisions, meeting minutes, etc. floating
around in multiple forums. We use the Developer Portal, Slack, JIRA,
GDrive, and GitHub for different purposes and we need to define what
information goes where.

## Attending

- @varl
- @mohammer5
- @amcgee

## What do we have today

- [wow-frontend](https://github.com/dhis2/wow-frontend)
- [Developer Portal](https://dhis2.github.io)
- [Slack](https://dhis2.slack.com)
- [JIRA](https://jira.dhis2.org)
- [GDrive](https://drive.google.com)

Proposals and ideas are spread out between JIRA, GDrive, and Slack. None
of which is explorable nor discoverable.

*JIRA* is good at tracking tasks which are to be done, but it is hopeless
to use for discussing ideas.

*Slack* is good for discussing ideas in (near) real-time, but is hopeless
for to discuss a specific issue over time as those which aren't on Slack
when the discussing happens probably won't know it ever happened unless
they read everything in their channel backlogs religiously.

*GDrive* has good collaboration features and works nicely for drafting
proposals. But unless the authors manually share, or put the document in
a shared space and then inform everyone else about its existence, it is
difficult for others to organically become aware of it. Comments and
resolving comments has its limitations when it comes to discussions
over time as well.

*Developer portal* is a developer resource to allow external/internal
developers to read more stable information and is a medium which is more
static in nature. The blog is a information channel where devs can read
interesting intel on a system after the fact, but it is hard to collect
input beforehand. The guide section is even more static in nature and
should only change as the established best practices changes.

*wow-frontend* use is to gather the Way of Work documentation for the
frontend team.

**Conclusion**: We need to consolidate where information is found to
make it easier to:

- _discover_ proposals and changes to the developer ecosystem
- _explore_ and _contribute_ to ideas which affect more than a single
  team
- _document_ decisions and have them easily accessible and transparent

## Consolidation effort

- Migrate the material in `dhis2/wow-frontend` to
  `dhis2/dhis2.github.io`

- Rename `dhis2/wow-frontend` to `dhis2/notes` (refer to
  [babel/notes](https://github.com/babel/notes) for an idea about the
  structure)

- By all means, discuss in Slack, but when/if you decide that it's
  something we should consider as a group, add a [proposal in GitHub
  Issues](https://github.com/dhis2/notes/issues/new).

  Example: https://github.com/dhis2/notes/issues/9

- Once a proposal has been outlined, and discussed, it is ready for a
  decision. This should be done in a meeting where the points outlined
  in the proposal are walked through. We can set up the agenda for a
  meeting in the form of a GitHub Issue.

  Example: https://github.com/dhis2/notes/issues/11

- The meeting should be recorded in a Markdown file in the correct
  directory (`YYYY/MM/DD.md`) with bulletpoints for each agenda topic
  and a conclusion for each topic.

- The meeting minute document is then raised as a PR, and once it has
  been discussed and approved we merge it and make the decision formal.


**Conclusion:**

- [`dhis2/wow-frontend`](https://github.com/dhis2/wow-frontend) is deprecated
  and integrated into the developer portal.

- [`dhis2/notes`](https://github.com/dhis2/notes) is for ideas, agendas, and decisions

- [Developer portal](https://github.com/dhis2/dhis2.github.io) is for
  long-lived information about topics which are interesting for
  DHIS2 developers (internal and external).

- [Google Drive](https://drive.google.com) is used at teams/developers
  own discretion.

- [Slack](https://dhis2.slack.com) is for real-time chat and
  collaboration, and used accordingly.

- Once we free ourselves from GitHub Pages to deploy the Developer
  Portal we will consolidate the repos which contain the portal and the
  notes, in essence merging: `dhis2/dhis2.github.io` and `dhis2/notes`.
