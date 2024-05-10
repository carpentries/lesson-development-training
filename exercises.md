---
title: Implementing Exercises
teaching: 10
exercises: 25
start: yes
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Display exercises and their solutions in a lesson site.


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How should exercises be presented in a lesson website?

::::::::::::::::::::::::::::::::::::::::::::::::::


Well-designed exercises are one of the most valuable resources for an instructor and
any time spent on this is well invested.

## Demo of Writing an Exercise

To create an exercise in The Carpentries Workbench,
you can use colon-delimited sections called 'fenced divs'.
In fact, [there are many types of boxes in the lesson infrastucture that use fenced divs](https://carpentries.github.io/sandpaper-docs/instructor/component-guide.html#callout-blocks).
In the Workbench, exercises are divided into two categories: _discussions_ (where the main task is for participants to discuss a topic or prompt) and _challenges_ (where the main task is a problem to be solved).

To start a challenge fenced div the line must contain at least 3 colons, then the `challenge` tag.
Then the content of the challenge is included on the following lines.
Finally, you can close the fenced div using another line with least 3 colons.

```markdown
:::::::::::::::::::::::::::::::::::::: challenge

### Challenge Title

Challenge text, code, and other information goes here

::::::::::::::::::::::::::::::::::::::::::::::::::

```

If you also want to include an expandable solution box for the challenge you can
add a solution fenced div within the challenge box.
The format is the same as for a challenge except the tag is `solution` instead.
Note the solutions can all be expanded for more accessible reading using the "Expand All Solutions"
option at the top of each episode.


```
:::::::::::::::::::::::::::::::::::::: challenge

### Challenge Title

Challenge text, code, and other information goes here

:::::::::::::: solution

### Solution Title

Solution text, code, and other information

:::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

```

For readability, you may want to have the length of the closing lines match the opening lines.
See in the above how the challenge and the nested solution's closing lines are similar lengths to the their corresponding opening lines.
For more information about creating exercises see the [Workbench Documentation for Exercises](https://carpentries.github.io/sandpaper-docs/episodes.html#exerciseschallenges).

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Formatting Exercises in a Lesson Site (15 minutes)

Using the approach demonstrated above,
format the exercise you designed previously as an exercise in your lesson site.


::::::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: More Practice with Fenced Divs (10 minutes)

Return to the bulleted list of prerequisite knowledge or skills you added to the `index.md` file of your lesson and
use fenced divs to display it in a formatted box with the `prereq` class.
Note that all lesson objectives in fenced divs will be combined into
one box at the top of each episode.


::::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::::: keypoints

- Exercises (and solutions) go in blocks using fenced divs in the lesson.

::::::::::::::::::::::::::::::::::::::::::::::::::


[^1]: [Kirschner et al. 2006](learners/reference.md#litref)
