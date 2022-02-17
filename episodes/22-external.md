---
title: Collaborating with newcomers
teaching: 30
exercises: 25
---

As with most open source and collaborative projects - you'll want to attract more effort to help
you maintain and improve the lesson. Often, this effort will come from people in the community you do not know beforehand, with varying sets of skills and amount of time to dedicate to your project. You should make an active effort to attract potential collaborators and try to make them all feel welcome and included as, in the words of Karl Fogel - the author of ["Producing Open Source Software"](ref), "if a project doesn’t make a good first impression, newcomers may wait a long time before giving it a second chance".
Fogel K. Producing Open Source Software: How to Run a Successful Free Software Project. Sebastopol, CA: O’Reilly Media; 2005. 

::::::::::::::::::::::::::::::::::::::: objectives

- Adjust a lesson repository to attract potential collaborators.
- Create and modify issue and pull request templates in GitHub.
- Identify strategies to encourage regular development and maintenance of a lesson.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What makes a project welcoming for newcomers?
- What information should I provide about the project to potential collaborators?
- How can I ensure regular progress on lesson development?

::::::::::::::::::::::::::::::::::::::::::::::::::

For collaborative lesson development projects it is important to spend the time on ‘external-facing’ project features, such as documentation, to make the project is welcoming for newcomers who may not have a deep grasp of the lesson or know all its existing problems. Such documentation will be useful to yourself and other team members as well, e.g. if you are trying to come back to the project after a break or are reusing it for a new collaboration in the future.

Your lesson documentation should contain the following information, which should be kept up to date:
- `README.md`- a README file is the first piece of documentation that people will land on when visiting your lesson repository. It should concisely explain what the lesson is about and who it is for, and contain links and pointers to further information, including:
  - Rendered version of the lesson: even though this is typically included in the `About` section of the repository, it is always useful to link to the URL where the rendered lesson is visible
  - Contact information: include email addresses or mailing lists or details on how to get in touch with the lesson maintainers
  - Contributing: this is an opportunity to list what kinds of contribution are sought and how to get involved in lesson development for new contributors. You can provide more details in a separate `CONTRIBUTING.md` file within the repository’s root directory and link to it from README. 
  - Credits/Acknowledgements: where appropriate, be sure to credit those who have helped in the lesson's development or inspired it, and/or any resources/templates that you have reused. You can also link to a separate file `AUTHORS.md` within the repository’s root directory, to list all the people who contributed to the lesson content (especially if this list starts to become rather large). 
  - Citation: it’s a very good idea to specify a reference to an appropriate academic publication so others can cite use of the lesson in their own publications and media. You can do this within a separate `CITATION.md` file within the repository’s root directory and link to it from README.
  - Licence: a short description of and a link to the lessons’s licence typically contained in a separate `LICENSE.md` file within the repository’s root directory.
- `CONTRIBUTING.md` - a file within the repository's root directory where you should provide detailed description of what kinds of contribution will be credited and in what ways. For example, at what point would someone be listed as an author and how you will credit contributions that are not recorded in the commit history of the project. The latter is particularly important for including newcomers who may not be proficient with the use of GitHub's features for collaborative work - such as Issues for managing bug reports, feature requests, and lists of future work; Mentions to reference team members/issues/commits/pull requests; Pull Requests to alert maintainers that new content is ready to be reviewed; Code Reviews to enable checks and discussions on contributed content - but could still provide valuable input and contributions.
- issue and pull request templates - consider setting up issue and pull request templates to help newcomers who may not have much experience working on team projects in GitHub. Such templates will prompt them to fill in answers to pre-set questions, which will help raise issues or submit pull requests in a way that’s clear, helpful and provides enough information for maintainers to act upon (without going back and forth to extract it). GitHub provides a range of default templates, but you can also [write your own](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository).

You may consider adding the following information to your documentation too:
- set-up guide for installing and rendering the lesson locally
- how to create and modify the pages in the lesson


::::::::::::::::::::::::::::::::::::::  challenge
## Exercise: preparing your repository for collaboration (15 minutes)

Spend some time doing **one of the following**:

1. Modify the `README.md` and `CONTRIBUTING.md` files in your repository
   to provide the relevant information for would-be contributors to your lesson:
   - the name(s) of the current developer(s), linked to their GitHub profile(s) (README)
   - contact information (README, CONTRIBUTING)
   - guidance on how people should contribute, and what kinds of contribution you are most interested in receiving (CONTRIBUTING)
   - links to any important background information (README)
   - links to any funding bodies or host institutes that are supporting the development of the lesson (README)
2. Create a new issue or pull request template, or modfy an existing one,
   to guide contributors on how best to begin collaborating with you on GitHub.

::::::::::::::::::::::::::::::::::::::::::::::::::

- listing lesson on [The Carpentries Help Wanted page](https://carpentries.org/help-wanted-issues/) and featuring in [the Incubator Lesson Spotlight](https://docs.carpentries.org/topic_folders/lesson_development/spotlight.html)
- noticing when something happens
  - using teams for mentioning multiple people
  - managing notifications
- making progress
  - scheduled co-working/sprinting sessions
  - Carpentries Maintainer co-working/lesson development co-working sessions
  - other strategies? blocking time in your calendar for issue triage/writing material?

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: planning to collaborate (10 minutes)

Use this time to plan how you will continue to make progress
with developing your lesson, and ensure that you are ready to respond to
external contributors when they arrive at your lesson.
This time is yours to do with as you think is best for yourself and your project,
but you might consider using it to do one or more of the following:

1. schedule a colesson development -working session with your collaborators,
   and/or mark the next community co-working session in your calendar.
2. ensure that your the notification settings are appropriately configured for
   your lesson repository.
3. contact The Carpentries team to ensure issues from your lesson will be
   included on the Help Wanted page.

::::::::::::::::::::::::::::::::::::::::::::::::::



:::::::::::::::::::::::::::::::::::::::: keypoints

- First key point. Brief Answer to questions. (FIXME)

::::::::::::::::::::::::::::::::::::::::::::::::::


