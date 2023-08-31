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

Developing a lesson is a project and, like most projects, it consists of multiple tasks. Keeping track of the list of tasks the team has to do, progress on each, prioritising tasks for future development, sprints and releases, etc., quickly becomes a non-trivial task in itself. Without a good project management framework, it can be hard to keep track of what’s done, or what needs doing, and particularly difficult to convey that to others in the team or share the responsibilities.

GitHub provides two project management tools for this purpose - **Milestones** and **Project Boards**.
Both Milestones and Project Boards implement an agile development/project management system
to help you keep track of different components of the project and their current status.
Milestones are good for [scrum-style project development and management](https://www.atlassian.com/agile/scrum) -
i.e. time-bound, structured iterations and working in short sprints on batches of issues. Project Boards implement
a [Kanban methodology](https://www.atlassian.com/agile/kanban) - good for managing continuous delivery and steady flow of work in a project.

Both Project Boards and Milestones are a way of organising issues into smaller "sub-projects" (i.e.
smaller than the "project" represented by the whole repository). When should you use one over the other?
Project Boards provide a way of visualising and organising the work on a higher level (e.g. more suitable for
project management tasks that are not time-bound). Milestones are a way to
organise lower-level tasks that have deadlines and progress of which needs to be closely tracked
(e.g. release management). How you organise and partition your project work is up to you and the size
of your project. For example, you could create a project per
milestone or have several milestones in a single project, and split milestones into shorter sprints.

### Milestones

A Milestone is a collection of issues to be worked on in a given time period. Milestones are good for
tracking progress as they provide an ordered list of issues which must all be resolved for the overall task to be
considered complete. Milestones work like labels - they mark and group issues that are expected to be closed at
some point in time.

The `Milestones` page in GitHub is accessible from the `Issues` page -
from there you can create a new milestone, see the percentage of issues completed for your milestones and their due dates.
You can also sort milestones by due date and prioritise issues within a particular milestone.
Back on the `Issues` page, you can assign issues to milestones and filter your issues by milestones.

### Project Boards
A Project Board (or Kanban board, from the Japanese word for 'card') uses columns and cards to keep track of tasks
- you break your project down into tasks which you write on cards, then move the cards between columns that describe the status of each task. Cards are usually small, descriptive and self-contained tasks that build on each other. Breaking a project down into clearly-defined tasks makes it a lot easier to manage and develop. GitHub project boards interact and integrate with the other features of the site such as issues and pull requests - cards can be added to track the progress of such tasks and automatically moved between columns based on their progress or status.

GitHub provides template boards that by default contain the three ‘basic’ columns, with pretty self-explanatory names:

- `To Do`
- `In Progress`
- `Done`

If you add an issue or pull request to a card in the board, it will automatically be moved to ‘Done’ for you when you close the issue or merge the pull request. One common extra column is `On hold` or `Waiting`. If you have tasks that get held up by waiting on other people (e.g. to respond to your questions) then moving them to a separate column makes their current state clearer.

You can also create a card without an issue. Such cards (or notes) can have detailed content like checklists or ideas
which are not necessarily suitable for inclusion in your issue tracker. However, GitHub also allows you to convert a card to an issue, should you wish to do so,
so you can add labels or detailed comments to it. Sometimes, a card you thought was simple and self-contained might turn out to be a bigger task than you anticipated - in that case, it is sensible to create new cards that reference the one they broke off from.

Once your project board has a large number of cards on it, you might want to begin prioritising them. Not all tasks are going to be equally important, and some will require others to be completed before they can even be begun. Common methods of prioritisation include:

- **Vertical position**: the vertical arrangement of cards in a column implicitly represents their importance. High-priority bugs go to the top of `To Do`, whilst tasks that depend on others go beneath them. This is the easiest one to implement, though you have to remember to correctly place cards when you add them.
- **Priority columns**: instead of a single `To Do` column, you can have two or more, for example - `To Do: Low Priority` and `To Do: High Priority`. When adding a card, you pick which is the appropriate column for it. You can even add a Triage column for newly-added issues that you’ve not yet had time to classify. This format works well for project boards devoted to bugs.
- **Labels**: if you convert each card into an issue, then you can label them with their priority - remember GitHub lets you create custom labels and set their colours. Label colours can provide a very visually clear indication of issue priority but require more administrative work on the project, as each card has to be an issue to be assigned a label. If you choose this route for issue prioritisation - be aware of accessibility issues for colour-blind people when picking colours.

::: callout

## Project Boards vs Milestones
For a good description of differences between the two, have a look at [this answer on StackOverflow](https://stackoverflow.com/questions/39591795/what-is-the-difference-relationship-between-github-projects-and-milestones).

A Project Board answers the question:

> *"What are we working on at the moment?"*

A Milestone answers the question:

> *"What is remaining to finish off this task?"*

:::

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: prioritising issues & planning work (15 minutes)

Use Project Boards and/or Milestones to prioritise issues and plan the first sprint and/or the first lesson release
with your team.

Depending on how many issues were registered on your repository, it is possible that you will not be able to work on
all the issues in the first sprint. As the development of your lesson progresses, any remaining unresolved issues can
be reconsidered and prioritised for another milestone and you can use a Project Board to plan them.

This process of receiving new issues and requirements, prioritisation, and working on them is naturally continuous -
with the benefit that at key stages your team is repeatedly re-evaluating what is important and needs to be worked on
which helps to ensure real concrete progress against project goals and requirements which may change over time.

::::::::::::::::::::::::::::::::::::::::::::::::::

## Project Governance

In addition to managing your project on a day-to-day basis, you should consider a governance model for your lesson to describe the ground rules of participation, the roles that project participants can take on and the process for decision making within the project. You may wonder why you'd ever need a formal governance process - after all, everyone in your team is collegial, polite and hard-working. However, even among the most harmonious teams you will likely realise you need an agreed way to make decisions and resolve conflicts when your team encounters their first real disagreement.

The moment your collaborator group exceeds 3 or 4 members (and fewer if the collaborators do not all know each other equally well at the outset) you should establish and document some kind of governance process. It will help mitigate any power imbalances which are expressed when one team member (or a group of team members) are more vocal and are able to dominate the decision-making process. It is advised to make these considerations early on, before your project grows too much and introducing structure and process into it becomes more difficult and complicated. Besides, if you do not establish these processes from the start, you are likely to discover the need to do so only when you first encounter disagreement within the team: a situation unlikely to provide perfect conditions for a discussion of governance.

Here are some aspects of governing a project that you should consider. These are borrowed from [the _Working in teams_ chapter](https://merely-useful.tech/py-rse/teams.html) of [_Research Software Engineering with Python_](https://merely-useful.tech/py-rse/index.html), a book on how to work productively in small teams where everyone is welcome:

- [Codes of Conduct](https://merely-useful.tech/py-rse/teams.html#teams-coc)
- [meeting rules](https://merely-useful.tech/py-rse/teams.html#teams-meetings)
- [decision-making process](https://merely-useful.tech/py-rse/teams.html#teams-martha)
- [handling conflict](https://merely-useful.tech/py-rse/teams.html#teams-conflict)
- [making all the above obvious to newcomers](https://merely-useful.tech/py-rse/teams.html#teams-documentation)

For some other examples and inspirations of governance processes, consider the following:

- [Martha’s Rules](https://journals.sagepub.com/doi/10.1177/088610998600100206) for discussing and deciding on issues in group meetings (if you cannot access the publication, see [Greg Wilson's explanation of Martha's rules](https://third-bit.com/files/2020/08/marthas/))
- [GitHub's Minimum Viable Governance](https://github.com/github/MVG) (MVG) for establishing a lightweight governance process into free and open source projects that are run in version control systems. In MVG decisions are made through consensus of the project maintainers or determined based on the maintainers' consideration of a number of factors in "good faith" (when explicit agreement of all maintainers cannot be reached). In reality, consensus-based governance can run you into trouble when you hit an issue where maintainers do not all agree but still want to make progress. Also, the definition of "good faith" is open to interpretation and leaves plenty of room for people, especially the powerful, to get away with acting in bad faith. A system based on voting and majorities may help you get around this issue. MVG is designed for a one organisation-many projects setup and is too elaborate for a single lesson project. However, it includes "boilerplate" template files for a steering committee, charter, governance, Code of Conduct documents, and language laying out a preference for consensus but with voting as a fallback, and other templates that may be helpful for those starting out and unsure about how to get on with establishing a governance process.
- [This list of resources related to community governance](https://docs.google.com/spreadsheets/d/1k8t1VPdcwKH7ZGaCA0q8NNxbFKQKkZGPth3nhfkKwAA/edit#gid=1287139202) from [The Center for Scientific Collaboration and Community Engagement](https://cscce.org) provides a collection of links to further reading material on this topic. It includes various guides, blog posts, and examples of community governance that may inform the discussions and decisions for your project.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercises: decision making process (15 minutes)

As a team read [Greg Wilson's explanation of Martha's rules on running decision making meetings](https://third-bit.com/files/2020/08/marthas/).

Discuss with your colleagues if it would work for your team and if not - what would you propose. Write down any
questions you may have for your trainers.

:::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::::: keypoints

- GitHub's **Milestones** and **Project Boards** can be used to effectively manage work sprints and a lesson development project as a whole, respectively.
- Make sure to consider and establish a governance model for your project early on - to describe the ground rules of participation and the process for decision making within the project.

:::::::::::::::::::::::::::::::::::::::
