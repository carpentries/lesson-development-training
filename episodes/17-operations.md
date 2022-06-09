---
title: How we operate
teaching: 25
exercises: 5
---

::::::::::::::::::::::::::::::::::::::: objectives

- Describe the life cycle of a lesson.
- Summarise the path a new lesson can take through The Carpentries Incubator and Lab.
- Connect with other members of the community.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What does The Carpentries lesson development ecosystem look like?
- What are the important milestones in the development of a new lesson?
- How can The Carpentries lesson development community help me complete my lesson?

::::::::::::::::::::::::::::::::::::::::::::::::::

Until now, this training has focused on the internals of a lesson development project.
Now it is time to consider the context in which this lesson development can take place.

## The Carpentries Lesson Development Ecosystem

[The Carpentries Incubator][carpentries-incubator] is a space for The Carpentries community
to collaborate on lessons.
It provides a single location where our community can come to 
find lessons that are being developed by the community,
and to create new lessons using The Carpentries Workbench.
Community members retain ownership of their lessons hosted in the Incubator,
while benefiting from the increased findability it gives to the lesson.

The Carpentries supports the lesson developer community working in the Incubator
with training (like this one),
communications designed to raise awareness of lesson projects within the community,
and platforms for the community to discuss and collaborate on lesson development.

The Carpentries also provides a space for community-developed lessons
to reside after the initial phases of development have been completed.
[The Carpentries Lab][carpentries-lab] provides a platform for open peer-review of lessons,
and hosts the collection of lessons that have passed through this review process. 
These peer-reviewed lessons can be considered ready to teach 
by any Instructor with sufficient knowledge of the topic.
In the future, this lesson review process may also be used to determine when a lesson
in the Incubator is ready to be incorporated into one of The Carpentries _Lesson Programs_,
the collection of lessons and curricula that can be taught in an official workshop for
Software, Library, or Data Carpentry.


## The Lesson Life Cycle

To make it easier for other community members to 
assess the current state of a lesson in the Incubator,
The Carpentries encourages lesson developers to indicate the status of their lesson 
by labelling its progress through a _lesson life cycle_:

![The life cycle of a lesson](fig/life_cycle.png){alt="Diagram of the life cycle of a
lesson in The Carpentries ecosystem. A lesson is proposed at the beginning of the 
pre-alpha stage. It enters alpha when it is taught for the first time. In beta, it is 
taught by other instructors. A full release of the lesson is made when it is stable. 
Pilot workshops take place during the alpha and beta phases. The Carpentries Lab hosts 
open peer review of lessons that have completed the beta phase."}

Each life cycle stage indicates the level of maturity of a lesson:

- **pre-alpha**: a first draft of the lesson is still being constructed.
- **alpha**: the lesson has been/is being taught by the original authors, but has not been fully tested.
- **beta**: the lesson is ready to be taught by instructors who have not been significantly involved in its developed to this point.
- **stable**: the lesson has been extensively tested by the authors and others. It can be considered broadly complete and unlikely to undergo any drastic changes without warning.

The life cycle stage of a lesson is displayed as a banner on the lesson site,
as a label on the lesson GitHub repository,
and alongside the lesson whenever it is shown on The Carpentries websites
and lesson listings.

The life cycle stage for a lesson is configured in the `config.yaml` file we
encountered when we were first introduced to [The Carpentries Workbench](07-infrastructure.md),
as a value for the `life_cycle` field. 
For new lesson repositories, this value is already set to 'pre-alpha', 
so you should not have to change it yet.

::: callout
### The `carpentry` Field

The `config.yaml` file also contains a `carpentry` field, which can be used to adjust
the styling applied to a lesson website e.g. to make it look like a lesson from the
Software, Library, or Data Carpentry Lesson Programs.

For community-developed lessons, where no official relationship exists with one of these
Lesson Programs, you should keep using the `incubator` setting, before potentially switching
over to another styling when the lesson moves e.g. into The Carpentries Lab.


:::::::::::


## Pilot Workshops

In line with [the importance we placed on evaluation of lesson content earlier in this training](03-audience.md),
the life cycle described above places considerable emphasis on 
the testing of lessons in **pilot workshops**.

For these pilot workshops to provide an effective evaluation of the lesson,
it is essential to seize the opportunity they provide to collect feedback and data.
For example, a pilot workshop offers a chance to answer questions like:

- How much time does it take to teach each section of the lesson?
- How much time is required for each exercise?
- What technical issues were encountered during the lesson?
- What questions did learners ask during the workshop? 
- Which parts of the lesson were confusing for learners?
- Which exercises could be improved to provide more information to the instructors?

[The pilot workshop notes template][pilot-notes-template] provides a starting point,
but it takes a lot of time and effort to keep track of all this information
during a pilot workshop. 
It can be helpful to assign this task to a member of the lesson development team,
who can dedicate themselves to observing the pilot and taking notes.
As soon as the pilot has finished,
it is a good idea to take some time to share the notes with the other lesson authors,
to reflect on and discuss the experience of teaching the lesson,
and to synthesise the lesson notes and any action items that come from this debrief 
into specific action items to improve the lesson.
These should be added as new issues on the lesson repository,
to help you keep track of the work that needs doing for the next iteration.

For beta pilot workshops, 
where the lesson is taught by instructors who have not yet made a major contribution to its development,
it is vital that instructors have the opportunity before the workshop 
to learn about the lesson from the authors,
and to debrief with the authors afterwards so that they can 
share their experience and observations about how the lesson could be further improved.


::: callout

## Hosting and Teaching Pilot Workshops

The Carpentries community handbook includes 
[guidance for community members who want to teach and/or host pilot workshops][handbook-pilot-workshops].

:::::::::::


## Connecting with the Lesson Developer Community

With over 100 lessons under development in The Carpentries Incubator,
the lesson developer community is thriving.
Connecting with this community can be a great way to
find collaborators to contribute to or test your lesson,
to stay up to date with the latest support provided to the community,
and to learn from the experience of others.

Here are a community activities and channels that you might be interested in joining:

- The `lesson-dev` channel on [The Carpentries Slack workspace](https://swc-slack-invite.herokuapp.com/). This is a platform for the community to ask questions and make announcements about lesson development. You could also browse the other channels on the workspace for any that are relevant to the topic of your lesson.
  - You may also find it helpful to create a new channel on Slack for discussion of your lesson. Chat channels like this can be valuable ways for a remote team to communicate and collaborate.
- [The `incubator-developers` list on TopicBox](https://carpentries.topicbox.com/groups/incubator-developers). The Carpentries Curriculum Team uses this mailing list to make relevant announcements to the community of lesson developers working in Incubator.
- The Carpentries Curriculum Team hosts monthly Lesson Development Coworking Sessions, which are a good opportunity to engage with other lesson developers and make regular progress on your project. The sessions are listed on [The Carpentries community calendar](https://carpentries.org/community/#community-events).


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: join relevant channels (5 minutes)

Use this time to explore the options listed above 
and join/subscribe to any communication channels that you find interesting.

::::::::::::::::::::::::::::::::::::::::::::::::::



:::::::::::::::::::::::::::::::::::::::: keypoints

- New lessons are developed in The Carpentries Incubator and reviewed in The Carpentries Lab.
- Teaching a lesson for the first time is an essential intermediate step in the lesson development process.
- The Carpentries lesson developer community shares their experience on multiple communication channels.

::::::::::::::::::::::::::::::::::::::::::::::::::


