---
title: Project Management and Governance
teaching: 30
exercises: 15
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Use GitHub features to help you with planning and managing your project.
- Prepare for a decision-making meeting between collaborators.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How can I use GitHub to manage a lesson development project?
- What strategies exist to help collaborators make decisions and govern an open source project?

::::::::::::::::::::::::::::::::::::::::::::::::::


## Project planning & management

Developing a lesson is a project and, like most projects, it consists of multiple tasks. 
Keeping track of the list of tasks the team has to do, progress on each, 
prioritising tasks for future development, sprints and releases, etc., 
quickly becomes a non-trivial task in itself. 
Without a project management tool/framework, it can be hard to keep track of what’s done, or what needs doing, 
and particularly difficult to convey that to others in the team or share the responsibilities.

Different tools and platforms exist to help you with project planning and management - 
for example, GitHub's [**Milestones**](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/about-milestones) and 
[**Projects**](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects), 
[Asana](https://www.asana.com), 
[Trello](https://www.trello.com), 
[Miro](https://miro.com/), 
even sticky notes on a white board. 
Different tools will work best for different teams of collaborators, 
but making sure you use any tool to plan and manage work on your lesson development project 
is better than making it up as you go along.

### Project Management in GitHub
Carpentries lessons are developed in GitHub so it is convenient (but not a must) to use GitHub's [**Milestones**](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/about-milestones) and [**Projects**](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) 
to help you keep track of different components of the project and their current status. 

Milestones are a way of organising issues on your project into smaller units of work (e.g. deliverables) that have deadlines and progress of which needs to be closely tracked (e.g. release management). 
Projects provide a way of visualising and organising the work on a higher level 
and are more suitable for project management tasks that are more continuous and not time-bound. 
While a Milestone is associated with a single repository, 
a Project can span over multiple Milestones and even different repositories within an organisation in GitHub. 

::: callout

## Milestones vs Projects
For a good description of differences between the two, have a look at [this answer on StackOverflow](https://stackoverflow.com/questions/39591795/what-is-the-difference-relationship-between-github-projects-and-milestones).

A Milestone answers the question:

> *"What is remaining to finish off this task?"*

A Project answers the question:

> *"What (tasks) are we working on at the moment?"*

:::

Milestones are good for managing time-bound, structured iterations and working in short sprints on batches of issues. 
Dedicated sprints seem to work well for lesson development, so we will have a look at how Milestones can help with this. 
We recommend you to also have a look at [GitHub's documentation on Projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) 
and see if they are suitable for your lesson development workflow.

### GitHub's Milestones

A Milestone is a collection of issues to be worked on in a given time period. 
Milestones are good for tracking progress as they provide an ordered list of issues 
which must all be resolved for the overall task to be considered complete. 
Milestones work like labels - 
they mark and group issues that are expected to be closed at some point in time.

The `Milestones` page in GitHub is accessible from the `Issues` or `Pull requests` pages -
from there you can create a new Milestone, 
set its description and due date, 
sort all Milestones by due date and see the percentage of issues completed for your Milestones.
Within an individual Milestone's page, 
you can see the list of associated issues and prioritise them by pointing to the left of an issue until the 'hand' pointer appears 
and then drag-and-dropping it to a new location in the list (with higher position in the list indicating higher priority). 
Back on the `Issues`/`Pull requests` page, 
you can assign issues/pull requests to a Milestone and filter your issues/pull requests by Milestones.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: prioritising issues & planning work (15 minutes)

Use Milestones to prioritise issues and plan the first sprint and/or the first lesson release
with your team.

Depending on how many issues were registered on your repository, it is possible that you will not be able to work on
all the issues in the first sprint. As the development of your lesson progresses, any remaining unresolved issues can
be reconsidered and prioritised for another sprint/milestone.

This process of receiving new issues and requirements, prioritisation, and working on them is naturally continuous -
with the benefit that at key stages your team is repeatedly re-evaluating what is important and needs to be worked on
which helps to ensure real concrete progress against project goals and requirements which may change over time.

::::::::::::::::::::::::::::::::::::::::::::::::::

## Project Governance

In addition to managing your project on a day-to-day basis, 
you should consider a governance model for your lesson to describe the ground rules of participation, 
the roles that project participants can take on and the process for decision making within the project. 
You may wonder why you'd ever need a formal governance process - 
after all, everyone in your team is collegial, polite and hard-working. 
However, even among the most harmonious teams you will likely realise you need an agreed way to make decisions 
and resolve conflicts when your team encounters their first real disagreement.

The moment your collaborator group exceeds 3 or 4 members 
(and fewer if the collaborators do not all know each other equally well at the outset) 
you should establish and document some kind of governance process. 
It will help mitigate any power imbalances which are expressed when one team member (or a group of team members) 
are more vocal and are able to dominate the decision-making process. 
It is advised to make these considerations early on, 
before your project grows too much and introducing structure and process into it becomes more difficult and complicated. 
Besides, if you do not establish these processes from the start, 
you are likely to discover the need to do so only when you first encounter disagreement within the team: 
a situation unlikely to provide perfect conditions for a discussion of governance.

Here are some aspects of governing a project that you should consider. 
These are borrowed from [the _Working in teams_ chapter](https://merely-useful.tech/py-rse/teams.html) of [_Research Software Engineering with Python_](https://merely-useful.tech/py-rse/index.html), 
a book on how to work productively in small teams where everyone is welcome:

- [Codes of Conduct](https://merely-useful.tech/py-rse/teams.html#teams-coc)
- [meeting rules](https://merely-useful.tech/py-rse/teams.html#teams-meetings)
- [decision-making process](https://merely-useful.tech/py-rse/teams.html#teams-martha)
- [handling conflict](https://merely-useful.tech/py-rse/teams.html#teams-conflict)
- [making all the above obvious to newcomers](https://merely-useful.tech/py-rse/teams.html#teams-documentation)

For some other examples and inspirations of governance processes, consider the following:

- [Martha’s Rules](https://journals.sagepub.com/doi/10.1177/088610998600100206)
  for discussing and deciding on issues in group meetings
  (if you cannot access the publication, see [Greg Wilson's explanation of Martha's rules](https://third-bit.com/files/2020/08/marthas/))
- [GitHub's Minimum Viable Governance](https://github.com/github/MVG) (MVG)
  for establishing a lightweight governance process into free and open source projects that are run in version control systems.
  - In MVG decisions are made through consensus of the project maintainers
    or determined based on the maintainers' consideration of a number of factors in "good faith"
    (when explicit agreement of all maintainers cannot be reached).
    In reality, consensus-based governance can run you into trouble
    when you hit an issue where maintainers do not all agree but still want to make progress.
    Also, the definition of "good faith" is open to interpretation
    and leaves plenty of room for people, especially the powerful,
    to get away with acting in bad faith.
  - A system based on voting and majorities may help you get around this issue.
    MVG is designed for a one organisation-many projects setup and is too elaborate for a single lesson project.
    However, it includes "boilerplate" template files for a steering committee, charter, governance, Code of Conduct documents,
    and language laying out a preference for consensus but with voting as a fallback,
    and other templates that may be helpful for those starting out and unsure about how to get on with establishing a governance process.
- [This list of resources related to community governance](https://docs.google.com/spreadsheets/d/1k8t1VPdcwKH7ZGaCA0q8NNxbFKQKkZGPth3nhfkKwAA/edit#gid=1287139202)
  from [The Center for Scientific Collaboration and Community Engagement](https://cscce.org)
  provides a collection of links to further reading material on this topic.
  It includes various guides, blog posts, and examples of community governance that may inform the discussions and decisions for your project.

::::::::::::::::::::::::::::::::::::::  discussion

## Exercises: decision making process (15 minutes)

These activities are intended to help you think about 
the human relationships between collaborators on a project
and how your interactions can influence the progress you make.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: spoiler

### For Teams of Collaborators

As a team read 
[the description of project governance for this training curriculum](https://github.com/carpentries/lesson-development-training/blob/main/GOVERNANCE.md).

Discuss with your colleagues which, if any, aspects of this would work for your team and which would not.
What model of governance and decision-making might work for your team?

If you have time remaining,
discuss what factors influence how much power each member of your team has
in the context of the project.
This could be "hard"/formalised power, 
e.g. project collaborators in more or less senior positions within the same workplace, 
and/or "soft"/informal, 
e.g. differences in the amount of time each collaborator has available for the project,
or different levels of expertise in the subject matter of the lesson,
or the lesson infrastructure and associated tools such as Git and GitHub.

Write down any questions you may have for your trainers.

(**Recommended reading**: the [_Dealing with Disruptive Behaviours_][noaa-ddb] resource
linked in the exercise for lesson developers working alone, below,
may also be helpful to ensure smoother project progress in your team.)

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: spoiler

### For Lesson Developers Working Alone

The [_Dealing with Disruptive Behaviours_][noaa-ddb] resource from 
the US National Oceanic and Atmospheric Administration (NOAA) Office for Coastal Management
provides guidance for meeting facilitators.
It includes examples of several common behaviours that can be disruptive to meetings
(and therefore to efficient progress on a project)
and advice for facilitators on how to intervene and mitigate them.

1. Open the _Dealing with Disruptive Behaviours_ resource, 
   select each behaviour, and read the descriptions.
2. Which of these behaviours do you recognise in yourself? 
   Put another way, which "character" ("Talkative Blowfish", "Apathetic Flounder", etc) do you most resemble?
3. Think about another project you work on where you are part of a team.
   Can you identify any of the disruptive behaviours in your colleagues?
   If so, can you find anything in the suggested interventions for these behaviours
   that could help you in your shared project?

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::::: keypoints

- Being intentional about task/project management for your lesson development project is better than making it up as you go along.
- Different tools and platforms exist to help you with project management - chose one that suits your team best.
- Dedicated work sprints seem to work well for lesson development and GitHub's **Milestones** can be used effectively to plan and manage such sprints.
- Make sure to consider and establish a governance model for your project early on - to describe the ground rules of participation and the process for decision making within the project.

:::::::::::::::::::::::::::::::::::::::

[noaa-ddb]: https://coast.noaa.gov/ddb/
