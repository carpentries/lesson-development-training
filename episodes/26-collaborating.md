---
title: Collaborating with people you already know
teaching: 75
exercises: 45
---

::::::::::::::::::::::::::::::::::::::: objectives

- Report and track issues with the GitHub interface.
- Review and provide feedback on contributions from collaborators.
- Prepare for a decision-making meeting between collaborators.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How can I use GitHub to manage a lesson development project?
- What communication channels are effective for a lesson development team?
- What strategies exist to help collaborators make decisions and govern an open source project?

::::::::::::::::::::::::::::::::::::::::::::::::::


In this episode we expand on how to use GitHub effectively among a group of known collaborators, building on top of tools and practices we introduced for working with newcomers. Everything you do to help your lesson be more attractive and informative to newcomers will benefit all collaborators. Here, we explore GitHub features to help you keep track of what needs doing on the lesson, making decisions and managing your project.

## Managing issues

**Issues** are GitHub's framework for managing issue/bug reports, feature requests, and lists of future work. They provide a single shared record of all the problems people have found with the lesson, and improvements that could be made, along with solutions and discussions around them. This helps the team to keep track of what they need to work on later, and reduces the chance of receiving redundant reports of issues you already know about.

When you create an issue, you can add a range of details to it. An issue can be assigned to a specific team member - this can be a helpful way to know who is currently working to fix an issue or a way to assign responsibility to someone to deal with it. You can assign one or more labels to issues to classify or group them. Labels can also be given colours, allowing you to see at a glance from the Issues page the state of your project. The default labels available in GitHub include:

- `bug` - indicates an unexpected problem or unintended behavior
- `documentation` - indicates a need for improvements or additions to documentation
- `duplicate` - indicates similar or already reported issues, pull requests, or discussions
- `enhancement` - indicates new feature requests, or if they are created by a lesson maintainer, indicate planned new features
- `good first issue` - indicates a good issue for first-time contributors
- `help wanted` - indicates that a maintainer wants help on an issue or pull request
- `invalid` - indicates that an issue, pull request, or discussion is no longer relevant
- `question` - indicates that an issue, pull request, or discussion needs more information
- `wontfix` - indicates that work won't continue on an issue, pull request, or discussion

Check the [GitHub documentaiton on Issues](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels) for the full reference.
We have already seen some of these labels - recall the `help wanted` and `good first issue` labels aimed at  newcomers to your project discussed in the previous episode. You can also create your own custom labels to help with classifying issues. There are no rules really about naming the labels - use whatever makes sense for your project. Some conventional custom labels include: `status:in progress` (to indicate that someone started working on the issue), `status:blocked` (to indicate that the progress on addressing issue is blocked by another issue or activity), etc.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercises: creating issues (15 minutes)

After your trial run,
you should have created a list of issues you identified with your lesson.
Open issues on the GitHub repository for your lesson,
for each item on that list.
Remember to add labels to each issue according to its type, priority, etc.
As you create them,
you may also want to assign these issues to a member of your lesson development team.


::::::::::::::::::::::::::::::::::::::::::::::::::


## Pull Requests

Although it is possible (for collaborators with sufficient access to the project)
to make changes to a lesson directly on the `main` branch of the repository,
doing so is not recommended:

1. It increases the likelihood of unintentional conflicts being created when two
   collaborators work on the same file simultaneously.
1. It does not provide an opportunity for changes to be checked and discussed 
   before they are included in the lesson. 
   This makes it much more likely that mistakes will be included in the lesson,
   and that the commit history of the project will include many
   changes made only to fix/polish/undo previous commits.
1. It prevents your team from benefiting from the powerful features that Git and GitHub
   provide to support and foster collaboration.

Instead, it is recommended practice to do most work in _branches_:
sets of changes that build on the work in the `main` branch (or another)
but are not included in that branch until they are explicitly _merged_ into it.
GitHub provides a way for this merging process to be managed,
by giving a platform for the changes to be described, discussed and reviewed,
before a decision is made to integrate or not integrate the changes 
in the default branch of the project and the associated lesson.

On GitHub, these units of discussion, review, 
and acceptance/rejection of the changes within a branch
are called _Pull Requests_.

:::::: callout

## Why "Pull Request"?

The name is slightly anachronistic now, because a project maintainer can often
manage the whole process of reviewing a contribution in GitHub's web interface,
but the term _Pull Request_ originates from the early days of GitHub, when
a contributor would be requesting that the project maintainer(s)
use Git to fetch or _pull_ the new branch to their local version of the project
repository, to further explore and test the changes before deciding whether to
merge them or not.

::::::::::::::


### Protecting `main`

As the maintainer of a project, you can enforce this workflow by
_protecting_ the default branch of the GitHub repository:
this will prevent anyone without _Admin_ access from committing changes directly to
that branch.

To activate this branch protection:

1. Open the _Settings_ tab of the repository and select _Branches_ in the left sidebar,
under _Code and automation_.
2. Click the "Add branch protection rule" button.
3. Type the name of the branch your GitHub Pages are being built from (`main`) 
   into the "Branch name pattern" box.
4. Check the "Require a pull request before merging" option, 
   but leave the others unchecked for now. 


### Submitting and Reviewing Pull Requests

The Trainers will collaborate on a demonstration of the process laid out below.


#### Pull Request Activity

_Note: This activity is designed to be carried out by two Trainers acting in two different roles:
"(S)" denotes the Pull Request Submitter role, "(R)" the Pull Request Reviewer._

1. \(S) Explore list of issues on repository, choose issue to fix, make note of issue number.
1. \(S) Edit a file to fix the issue, commit changes to a new branch with an appropriate name.
        Ensure that the changes include some typo etc that the Reviewer
        will be able to comment on and/or suggest a fix/improvement to.
1. \(S) Show how to open a pull request from that new branch to `main`.
1. \(S) In Pull Request description, reference the number of the issue being fixed, 
        using a keyword ("Fixes", "Resolves") to ensure automatic closure.
1. \(S) Demonstrate how to mark the PR as a draft, 
        and then how to mark as it as ready for review.
1. \(S) Request a review from the Pull Request Reviewer.
1. \(R) Open the new Pull Request in GitHub.
1. \(R) Explore the diff of the PR, 
        by opening the _Files changed_ tab and talking through the display.
1. \(R) Comment on a line in the diff.
1. \(R) Suggest a change to the diff, 
        using the "Add suggestion" button or three backticks marked `suggestion`.
1. \(R) Complete your review by adding some summary text and selecting "Request changes".
1. \(R) Return to _Conversation_ tab, 
        to show how the PR thread looks after the review has been submitted.
1. \(S) Navigate to PR and the _Files changed_ tab.
1. \(S) Respond to Reviewer's comment(s), accept their suggested changes
        (draw attention to the option to batch multiple suggestions into a single commit).
1. \(S) Return to the _Conversation_ tab and request a new review from the Reviewer.
1. \(R) Look again at the PR diff (_Files changed_) 
        and ensure that requested changes have been made.
1. \(R) Approve the PR.
1. \(R) Thank the Submitter for their contribution.
1. \(R) Merge the PR.
1. \(R) Navigate to issue listing to confirm that the relevant issue has been 
        automatically closed.


:::::: challenge

### Practice with Pull Requests (15 minutes)

In breakout groups, assign yourselves the role of Submitter (S) and Reviewer (R),
and repeat the process described above by completing the steps below.
If anythere are any issues open on the repository that can be solved very quickly,
feel free to address those with this exercise.
Otherwise, the Submitter can open a Pull Request to make simple changes:
typo fixes, or some completely arbitrary changes to a file.
If the changes made for the exercise are not improvements to the lesson,
the Reviewer should follow all the steps but close the PR at the end instead of merging it.

1. \(S) Edit a file and commit the changes to a new branch.
2. \(S) Open a new Pull Request from this new branch to `main`.
        If your PR will fix an open issue on your repository,
        include "Fixes #X" at the start of the PR description,
        where _X_ is the issue number.
3. \(S) Request a review from the Reviewer.
4. \(R) Review the PR, making comments and suggesting changes as appropriate.
        When you have finished, approve the PR or request changes, based on your review.
5. \(S) Respond to any comments from the Reviewer and/or, if any changes were requested,
        make those and re-request a review when you have finished.
6. \(R) When all changes have been made to your satisfaction,
        approve the PR, thank the Submitter for their contribution,
        and merge the PR
        (Or close it if the changes were made for practice but should not
        be included in the actual lesson.)

::::::::::::::::


## Managing communication

Having an open, publicly-visible list of all the issues with your project is a helpful way of letting people know you are aware of issues and you are working on them. This can indicate to an external audience that the project is active. 
It also provides you and your collaborators with an "at a glance" view of the state of the project, making it easier to prioritise future work.

As we have seen in the previous episode, GitHub's notifications framework **Mentions** plays an important part in communicating between collaborators and is used as a way of alerting team members of activities and referencing one issue/comment/pull requests from another.

[Slack](https://slack.com/) is commonly used in the Carpentries community for quick, day-to-day message exchange among teams. You can create your own [Slack workspace for free](https://slack.com/intl/en-gb/) or create a channel for your lesson development project under [the Carpentries public Slack workspace](https://swcarpentry.slack.com/). Note that the Carpentries Slack is an enterprise workspace so all messages and files will be retained and no messages will be lost (for free workspaces only the most recent 10,000 messages can be viewed and searched and file storage limit is 5 GB). 

Collaborators can also use other platforms to discuss lesson development or receive contributions from newcomers who are not yet fluent in using GitHub's systems of communication. The Carpentries can assist with creating a mailing list specific to the development of your lesson on their [TopicBox](https://carpentries.topicbox.com/) platform for managing threaded email discussions. Also make sure to join the [Incubator lesson developers mailing list](https://carpentries.topicbox.com/groups/incubator-developers) on TopicBox to keep an eye on announcements and discussions relating to lesson development in general within the Carpentries community.

Meeting minutes are a useful way of providing a permanent record of the purpose of a meeting and what was talked about, including any decisions made or actions taken, that can be referred back to for any follow-ups. Recording meeting minutes does not have to be hard - remember that you are part of a team and there are many platforms that allow collaborative note taking. The Carpentries provides [CodiMD](https://codimd.carpentries.org/) and [Etherpad](https://pad.carpentries.org/) instances as two options for taking shared notes, widely used at workshops for sharing pieces of code, references and notes between instructors and learners. For some advice on holding effective meetings, see [the _Meetings, meetings, meetings_ section of Teaching Tech Together](https://teachtogether.tech/en/index.html#s:meetings) by Greg Wilson.

## Project management

Developing a lesson is a project and, like most projects, it consists of multiple tasks. Keeping track of the list of tasks the team has to do, progress on each, prioritising tasks for future development, sprints and releases, etc., quickly becomes a non-trivial task in itself. Without a good project management framework, it can be hard to keep track of what’s done, or what needs doing, and particularly difficult to convey that to others in the team or share the responsibilities.

GitHub's project management framework **Project Board** is a tool for keeping track of all the different components of a project, and what their current status is. It does this using columns and cards - you break your project down into tasks which you write on cards, then move the cards between columns that describe the status of each task. Cards are usually small, descriptive and self-contained tasks that build on each other. Breaking a project down into clearly-defined tasks makes it a lot easier to manage and develop. GitHub project boards interact and integrate with the other features of the site such as issues and pull requests - cards can be added to track the progress of such tasks and automatically moved between columns based on their progress or status.

GitHub provides template boards that by default contain the three ‘basic’ columns, with pretty self-explanatory names:

- `To Do`
- `In Progress`
- `Done`

If you add an issue or pull request to a card in the board, it will automatically be moved to ‘Done’ for you when you close the issue or merge the pull request. One common extra column is `On hold` or `Waiting`. If you have tasks that get held up by waiting on other people (e.g. to respond to your questions) then moving them to a separate column makes their current state clearer. 

You can also create a card without an issue. Such cards (or notes) can have detailed content like checklists. GitHub also allows you to convert a card to an issue so you can add labels or detailed comments to it. Sometimes, a card you thought was simple and self-contained might turn out to be a bigger task than you anticipated - in that case, it is sensible to create new cards that reference the one they broke off from.

Once your project board has a large number of cards on it, you might want to begin priorisiting them. Not all tasks are going to be equally important, and some will require others to be completed before they can even be begun. Common methods of prioritisation include:

- **Vertical position**: the vertical arrangement of cards in a column implicitly represents their importance. High-priority bugs go to the top of `To Do`, whilst tasks that depend on others go beneath them. This is the easiest one to implement, though you have to remember to correctly place cards when you add them.
- **Priority columns**: instead of a single `To Do` column, you can have two or more, for example - `To Do: Low Priority` and `To Do: High Priority`. When adding a card, you pick which is the appropriate column for it. You can even add a Triage column for newly-added issues that you’ve not yet had time to classify. This format works well for project boards devoted to bugs.
- **Labels**: if you convert each card into an issue, then you can label them with their priority - remember GitHub lets you create custom labels and set their colours. Label colours can provide a very visually clear indication of issue priority but require more administrative work on the project, as each card has to be an issue to be assigned a label. If you choose this route for issue prioritisation - be aware of accessibility issues for colour-blind people when picking colours. 

## Project governance

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
- [GitHub's Minimum Viable Governance](https://github.com/github/MVG) (MVG) for establishing a lightweight governance process into free and open source projects that are run in version control systems. In MVG decisions are made through consensus of the project maintainers or determined based on the maintainers' consideration of a number of factors in "good faith"" (when explicit agreement of all maintainers cannot be reached). In reality, consensus-based governance can run you into trouble when you hit an issue where maintainers do not all agree but still want to make progress. Also, the definition of "good faith" is open to interpretation and leaves plenty of room for people, especially the powerful, to get away with acting in bad faith. A system based on voting and majorities may help you get around this issue. MVG is designed for a one organisation-many projects setup and is too elaborate for a single lesson project. However, it includes "boilerplate" template files for a steering committee, charter, governance, Code of Conduct documents, and language laying out a preference for consensus but with voting as a fallback, and other templates that may be helpful for those starting out and unsure about how to get on with establishing a governance process.
- [This list of resources related to community governance](https://docs.google.com/spreadsheets/d/1k8t1VPdcwKH7ZGaCA0q8NNxbFKQKkZGPth3nhfkKwAA/edit#gid=1287139202) from [The Center for Scientific Collaboration and Community Engagement](https://cscce.org) provides a collection of links to further reading material on this topic. It includes various guides, blog posts, and examples of community governance that may inform the discussions and decisions for your project.

:::::::::::::::::::::::::::::::::::::::: keypoints


- GitHub's features **Issues**, **Mentions** and **Project Boards** can all be used to effectively communicate in a team of collaborators and manage a lesson development project.
- Slack and emailing lists provide communication channels outside of GitHub - for quick day-to-day messaging and more permanent discussions around lesson issues and development, respectively.
- Make sure to establish a governance model for your project early on - to describe the ground rules of participation and the process for decision making within the project.


::::::::::::::::::::::::::::::::::::::::::::::::::


