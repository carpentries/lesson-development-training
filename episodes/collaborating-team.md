---
title: Collaborating with Your Team
teaching: 30
exercises: 45
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Report and track issues with their lesson using the GitHub interface.
- Review and provide feedback on contributions from collaborators using the GitHub interface.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How can I use GitHub to manage (report, assign, track, prioritise) tasks of a lesson development project?
- What communication channels are effective for a lesson development team?
- How can I use GitHub to manage contributions from collaborators?

::::::::::::::::::::::::::::::::::::::::::::::::::


In this episode we expand on how to use GitHub effectively among a group of known
collaborators on an open source lesson development project, setting the stage for introducing tools and practices for
working with newcomers. Here, we explore GitHub features to help you keep track of what needs doing on
the lesson, manage contributions and prioritise work. Making decisions and managing your project as a whole will
be covered in a follow-up episode on [project management](./project-management.html).
Collaboration skills covered in this and follow-up episodes are transferable
to any similar open source project you may be involved with.

## Managing Issues

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
You can also create your own custom labels to help with classifying issues.
There are no rules really about naming the labels - use whatever makes sense for your
project. Some conventional custom labels include: `status:in progress` (to indicate that
someone started working on the issue), `status:blocked` (to indicate that the progress on
addressing the issue is blocked by another issue or activity), etc.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: creating issues (15 minutes)

After your trial run,
you should have created a list of issues you identified with your lesson.
Open issues on the GitHub repository for your lesson,
for each item on that list.
Remember to add labels to each issue according to its type, priority, etc.
As you create them,
you may also want to assign these issues to a member of your lesson development team.


::::::::::::::::::::::::::::::::::::::::::::::::::


## Managing Contributions

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

The term _Pull Request_ originates from the early days of GitHub, when
a contributor would be requesting that the project maintainer(s)
use Git to fetch (download) their branch and merge the changes
into the main branch of the project.
In the terminology of Git, this combination of fetching and merging a set of changes
is called _pulling_.
The name Pull Request is slightly anachronistic now, because a project maintainer can often
manage the whole process of reviewing a contribution in GitHub's web interface.

Note: A common nickname for a _Pull Request_ is PR or PRs for _Pull Requests_.

::::::::::::::


### Submitting and Reviewing Pull Requests on GitHub

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
        using a keyword "Fixes #X" or "Resolves #X" (where _X_ is the issue number) to ensure automatic closure.
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
If there are any issues open on the repository that can be solved very quickly,
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

:::::::::::::::::::::::::::::::: callout

### Protecting `main` Branch

Repository administrators can enforce this workflow by
_protecting_ the default branch of the GitHub repository:
requiring anyone without _Admin_ access to submit changes by pull request
instead of committing changes directly to `main`.

The GitHub documentation provides 
[more information about this feature and other branch protection rules](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule).

::::::::::::::::::::::::::::::::::::::::


:::::: callout

## Effective review comments are a learned skill

Making effective review comments in a PR is something you will get better at with practice - here is some general guidance to help with reviewing a PR from a collaborator:

- Make sure your review comments are specific and actionable.
- Make it clear in the comment what you want changed as part of a PR and, ideally, provide a concrete suggestion.
- Only request changes if the content is wrong or hard to understand (remember, different does not always mean better).
- If a conversation on a PR hasn’t been resolved by one or two back-and-forth exchanges, consider scheduling a meeting to discuss further.
- Good reviews have empathy - consider the contributor's feelings, identify positives and try not to be judgemental.
- Aim for improved/better rather than perfect.

::::::::::::::::


## Managing Communication

Having an open, publicly-visible list of all the issues with your project is a helpful way of letting people know you are aware of issues and you are working on them. This can indicate to an external audience that the project is active.
It also provides you and your collaborators with an "at a glance" view of the state of the project, making it easier to prioritise future work.

GitHub provides a useful notification feature for collaborative work - _mentions_.
The mention system notifies team members when somebody else references them
in an issue, comment or pull request -
you can use this to notify people when you want to check a detail with them,
or let them know something has been fixed or changed
(much easier than writing out all the same information again in an email!).
You can use the mention system to notify individual GitHub accounts
or whole teams (when you need to mention multiple people at once and it is not practical to list them all individually).
Typing `@` in GitHub will bring up a list of all accounts and teams linked to the repository that can be "mentioned".

[Slack](https://slack.com/) is commonly used in the Carpentries community for quick, day-to-day message exchange among teams. You can create your own [Slack workspace for free](https://slack.com/intl/en-gb/) or create a channel for your lesson development project under [the Carpentries public Slack workspace](https://carpentries.slack.com/). Note that the Carpentries Slack is an enterprise workspace so all messages and files will be retained and no messages will be lost (for free workspaces only the most recent 10,000 messages can be viewed and searched and file storage limit is 5 GB).

Collaborators can also use other platforms to discuss lesson development or receive contributions from newcomers who are not yet fluent in using GitHub's systems of communication. The Carpentries can assist with creating a mailing list specific to the development of your lesson on their [TopicBox](https://carpentries.topicbox.com/) platform for managing threaded email discussions. Also make sure to join the [Incubator lesson developers mailing list](https://carpentries.topicbox.com/groups/incubator-developers) on TopicBox to keep an eye on announcements and discussions relating to lesson development in general within the Carpentries community.

:::::::::::::::::::::::::::::::::::::::: keypoints

- GitHub's features **Issues**, **Pull Requests** and **Mentions** can all be used to transparently and effectively communicate and collaborate in a team working on a lesson development project.
- Slack and emailing lists provide communication channels outside of GitHub - for quick day-to-day messaging and more permanent discussions around lesson issues and development, respectively.

::::::::::::::::::::::::::::::::::::::::::::::::::
