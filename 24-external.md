---
title: Collaborating with newcomers
teaching: 30
exercises: 25
---

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

So far, the focus of the training was on lesson development skills. In this section, we will learn more about the skills and tools you can use to become an effective collaborator on an open source lesson development project and how to employ your lesson development skills in a team environment. Collaboration skills covered here are transferrable to any similar open source project you may be involved with. 

You may start working on projects by yourself or with a small group of collaborators you already know, but open source projects in the Carpentries community often grow beyond that small group. Community collaboration is the cornerstone of The Carpentries - all curricula and various programmes are developed together by the community members across borders, domains and backgrounds. Most initiatives are done through community consultation and collaboration is used as a pathway to empower people, give members a sense of purpose in the community and realise shared goals.

Collaboration helps bring different perspectives to solving a problem and share the load of the required work to develop, pilot, and, later on, maintain the lesson. People drop in and out of projects for various reasons and their levels of involvement may vary over time due to other commitments - for this reason it is worth taking time from the outset to make a project welcoming for newcomers in order to achieve a steady number of people working on your project at any time. You should plan to make it easy for new collaborators to join, to set up a local workspace so that they can contribute, help them find tasks so that they know what to contribute, and make the contribution process clear so that they know how to contribute. You also want to make it easy to give people credit for their work on your project as well as for others to reuse and give credit to your project. From this episode on, we cover best practices for collaboration and tools available to us achieve it.

## Documenting your lesson

For collaborative projects, it is important to spend the time on ‘external-facing’ features, such as documentation, to make the project as welcoming and as easy to get involved in as possible for newcomers who may not have a deep grasp of the project or know all its existing problems. Such documentation will be useful to yourself and other team members at well, e.g. if you are trying to come back to the project after a break or are reusing it for a new collaboration in the future.

Your lesson documentation should contain the following information, which should be kept up to date.

### Description of the project - `README` file

`README`, `README.txt` or `README.md` is a plain text or Markdown file located in the project's root directory representing the default landing or home page for repositories in GitHub (and similar project repositories) by convention. It represents the first piece of documentation that people will see when visiting your lesson repository, hence it should concisely explain what the lesson is about and who it is for, and contain links and pointers to further information. For example, `README` should include:

- **lesson title**
- **lesson description**
- **rendered version of the lesson** - even though this is typically included in the `About` section of the repository, it is always useful to link to the URL where the rendered lesson is available
- **contact information** - include up-to-date email addresses or mailing lists or other details on how to get in touch with the lesson maintainers
- **contributing information** - this is an opportunity to list what kinds of contribution are sought and how to get involved in lesson development for new contributors. You can provide more details in a separate `CONTRIBUTING` file within the repository’s root directory and link to it from `README`
- **credits/acknowledgements** - make sure to credit those who have helped in the lesson's development or inspired it, and/or any resources/templates that you have reused. You can also link to a separate `AUTHORS.md` file within the repository’s root directory to list all the people who contributed to the lesson content (if this list starts to become too large to include in the `README` itself)
- **citation** - a convention is to include the citation information for your lesson in a separate `CITATION` file within the repository’s root directory (and link to it from `README`) so others can cite the use of the lesson in their own publications and media and it can also be automatically discovered by other applications. Citation can be a Digital Object Identifier (DOI) issued by a reputable DOI-issuing repository such as [Zenodo](https://zenodo.org/), which should be obtained as a permanent identifier as soon as your lesson reaches the beta stage, or an appropriate academic publication once your lesson becomes stable and is peer-reviewed. 
Citation can be contained in a plain text file (`CITATION`, `CITATION.txt`), a Markdown file (`CITATION.md`), or in the recently adopted [Citation File Format](https://github.com/citation-file-format/citation-file-format) (`CITATION.cff`). The CFF is defined using [YAML](https://yaml.org/spec/1.2.2/) (which we already encountered in the `config.yaml` file for the lesson website) and is now [the recommended way of storing citations in GitHub](https://github.blog/2021-08-19-enhanced-support-citations-github/). Advantages of using CFF are that GitHub will automatically show the citation information in the sidebar, making it more visible and accessible for visitors to your repository. In addition, metadata from `CITATION.cff` files will automatically be used by [Zenodo](https://zenodo.org/) when registering the DOI for your lesson/project. CFF metadata is also recognised by the [Zotero reference manager](https://www.zotero.org/).
- **license** - a short description of and a link to the lesson’s license typically contained in a separate `LICENSE`, `LICENSE.txt` or `LICENSE.md` file within the repository’s root directory. The lesson repository created from the Carpentries lesson template already contains a default `LICENSE.md` file, but you should modify this to more accurately describe how the lesson content can be re-used by others.

### Instructions for contributors - `CONTRIBUTING` file

`CONTRIBUTING`, `CONTRIBUTING.txt` or `CONTRIBUTING.md` is a text or Markdown file within the repository's root directory where you should provide detailed description of the ways people can send their contributions, what kinds of contribution will be credited and in what ways. For example, at what point would someone be listed as an author and how you will credit contributions that are not recorded in the commit history of the project. The latter is particularly important for newcomers who may not be proficient with the use of GitHub's features for collaborative work, such as issues, mentions, pull requests and code review, but could still provide valuable input and contributions.

Carpentries lesson repositories already have a generic Carpentries `CONTRIBUTING.md` file to get you started. You should review it and, if need be, modify it to fit your team's needs and way of working. For example, you may want to expand on what contributions you are *not* looking for if your lesson already contains more material than can be covered in a typical workshop. You can also detail all channels on which you are willing to receive contributions on if they are different from the defaults included in the file.

### Issue and pull request templates

Consider setting up issue and pull request templates to help newcomers who may not have much experience working on collaborative projects in GitHub. Such templates can provide a structure for the issue/pull request description, and/or prompt them to fill in answers to pre-set questions. Both can help contributors raise issues or submit pull requests in a way that is clear, helpful and provides enough information for maintainers to act upon (without going back and forth to extract it). GitHub provides a range of default templates, but you can also [write your own](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository).

### Other documentation

Once you have set up the basic documentation about your lesson, you may consider adding the following useful information to your documentation too:

- set-up guides for installing and rendering the lesson locally. In most cases, a link to [The Carpentries Workbench documentation](https://carpentries.github.io/sandpaper-docs/) will be sufficient.
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

Groups of collaborators taking this training together should discuss first how they will assign these tasks between them.
::::::::::::::::::::::::::::::::::::::::::::::::::

## Collaborating on a lesson

### Boosting the visibility and attracting new collaborators

In addition to having the complete documentation in the lesson repository, The Carpentries community provides a number of ways to further raise the visibility of the lesson among the broader community and encourage community members to contribute to its further development. For example:

  - listing issues from the lesson repository on [The Carpentries Help Wanted page](https://carpentries.org/help-wanted-issues/)
  - featuring your lesson in [the Incubator Lesson Spotlight](https://docs.carpentries.org/topic_folders/lesson_development/spotlight.html)
  - writing a blog post about the lesson for [The Carpentries Blog](https://carpentries.org/blog), and/or attending a community discussion call to promote the lesson
  - advertising the lesson at various Carpentries mailing lists - e.g. [general discussion](https://carpentries.topicbox.com/groups/discuss), [instructors](https://carpentries.topicbox.com/groups/instructors), regional communities or specific curriculum lists

You should also consider including your lesson in [Hacktoberfest](https://hacktoberfest.digitalocean.com/) and similar wider community open source events aimed at encouraging people to contribute to open source projects periodically throughout the year.

### Issue labelling for newcomers

You can encourage contributions to your lesson from newcomers by using specific labels on issues to highlight suitable opportunities to help. Apply the `good first issue` or `help wanted` labels to issues in your repository to indicate that the maintainers will particularly welcome help or pull requests fixing such issues.

### Noticing when something happens

GitHub implements a comprehensive [notifications system](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications) to keep you up-to-date with activities in the lesson repository. GitHub also provides an additional useful notification feature for collaborative work - **Mentions**. The mention system notifies team members when somebody else references them in an issue, comment or pull request - you can use this to notify people when you want to check a detail with them, or let them know something has been fixed or changed (much easier than writing out all the same information again in an email!). You can use the mention system to link to individual GitHub accounts or whole teams for mentioning multiple people. Typing `@` in GitHub will bring up a list of all accounts and teams linked to the repository that can be "mentioned".

Check out [GitHub's documentation on setting notifications on individual repository](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications#configuring-your-watch-settings-for-an-individual-repository). You can choose whether to watch or unwatch an individual repository, or can choose to only be notified of certain event types such as issues, pull requests, mentions, etc.


### Making progress

The following practices have been shown to help maintain steady progress with lesson development:

  - being responsive to notifications about activities and mentions
  - scheduling regular co-working/sprinting sessions with team members
attaching your sprint sessions to other open source community activities, which may offer goodies, rewards and prizes for participants, can provide motivation and activity spikes
  - working alongside other members of The Carpentries community at Maintainer or lesson development co-working sessions
  - blocking time in your calendar for issue triage/solo material writing
  - planning lesson pilots in advance to help set targets


Make sure to join the [Incubator lesson developers mailing list](https://carpentries.topicbox.com/groups/incubator-developers) to keep an eye on announcements and discussions relating to lesson development in the Carpentry community.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: planning to collaborate (10 minutes)

Use this time to plan how you will continue to make progress
with developing your lesson, and ensure that you are ready to respond to
external contributors when they arrive at your lesson.
This time is yours to do with as you think is best for yourself and your project,
but you might consider using it to do one or more of the following:

1. schedule a lesson development co-working session with your collaborators,
   and/or mark the next community co-working session in your calendar.
2. ensure that your the notification settings are appropriately configured for
   your lesson repository.
3. contact The Carpentries team to ensure issues from your lesson will be
   included on the Help Wanted page.

::::::::::::::::::::::::::::::::::::::::::::::::::



:::::::::::::::::::::::::::::::::::::::: keypoints

- *"If a project doesn’t make a good first impression, newcomers may wait a long time before giving it a second chance" - Karl Fogel, the author of ["Producing Open Source Software: How to Run a Successful Free Software Project"](https://www.oreilly.com/library/view/producing-open-source/0596007590/)*.
- You should make an active effort to attract potential collaborators and try to make them all feel welcome and included. [The Carpentries Help Wanted page](https://carpentries.org/help-wanted-issues/) and featuring in [the Incubator Lesson Spotlight](https://docs.carpentries.org/topic_folders/lesson_development/spotlight.html) can boost the visibility of your lesson. Creating the appropriate documentation and using GitHub features such as labels, and issue/pull request templates will help lower the barriers for contributions to your project.
- Scheduling regular co-working sessions, blocking time in the calendar for issue triage, and setting and being responsive to GitHub notifications will ensure regular progress on the lesson.

::::::::::::::::::::::::::::::::::::::::::::::::::

