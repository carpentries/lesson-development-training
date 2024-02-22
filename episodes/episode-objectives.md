---
title: "Defining Episode Objectives"
teaching: 5
exercises: 30
---


:::::::::::::::::::::::::::::::::::::: questions

- How should objectives be written for a smaller part of a whole lesson?
- How are objectives added to an episode page?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Define learning objectives for a section of a lesson.
- Format objectives in the individual pages of a lesson website.

::::::::::::::::::::::::::::::::::::::::::::::::

In _Defining Lesson Objectives_,
you created a list of the learning objectives for your lesson as a whole.
This process is helpful as a way to set the end goal and,
coupled with the expected prior knowledge of the target audience you identified,
describe the scope of the lesson.

We can use the same approach for the individual episodes of a lesson,
defining objectives for the episode to make clear what we intend to teach in that section.
Defining these objectives _before writing the episode content_ helps us to:

- stay focused in the episode, without spending time on non-essential topics
- determine whether learners are attaining the skills we wish to teach them
  (we will discuss this more in the next two episodes)
- summarise the skills the learner can expect to gain by following this section of the lesson

As before, here are some recommendations to help you define these episode-level objectives:

- Aim for 2-4 objectives per episode. 
  If you need to write more than that,
  consider breaking this section down into multiple episodes.
- To ensure your episode content aligns with the overall goals for the lesson,
  try to identify which lesson-level objective(s) your episode
  will contribute to.
- In the context of the previous recommendation,
  consider how the objectives for your episode fit as a
  component of the higher-level skills/understanding defined
  in the lesson-level objective(s).

::: challenge

### Exercise: define objectives for your episode (30 minutes)

1. Using the same approach as you did for your whole-lesson objectives,
   define a set of SMART objectives for your chosen episode. (15 minutes)
1. Add this list of objectives to replace
   the `TODO` in the `objectives` fenced div of your episode file (5 minutes)
1. Compare your list with those created by your collaborators on the lesson:
    - are there any gaps in these objectives,
      i.e. anything that should be covered in these episodes but is not captured in the objectives?
    - are there any overlaps, i.e. anything that looks like it will be covered more than once?
1. As a group, discuss how you will address any problems identified in the previous step,
   and edit your objectives accordingly.

:::::: solution

After you have defined the episode objectives, you can add them to the `objectives` div as follows:

```markdown
::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- objective 1
- objective 2
- ...

::::::::::::::::::::::::::::::::::::::::::::::::
```

::::::

:::


::: callout

### Full List of Fenced Divs

[The Workbench Component Guide][component-guide] provides a full list of
all the different classes of fenced div that can be included using the lesson infrastructure.
The guide specifies which divs are required for an episode
(`objectives`, `questions`, and `keypoints`),
and which are optional.

:::

Now that we have defined objectives for our episodes,
we can start working on the next step in developing an effective lesson:
designing exercises that will assess whether a learner has learned what you aimed to teach them.

::::::::::::::::::::::::::::::::::::: keypoints

- Objectives can be defined for episodes within a lesson, to guide individual steps along the pathway of the lesson.
- Objectives should be included in each episode page as an `objectives` fenced div.

::::::::::::::::::::::::::::::::::::::::::::::::
