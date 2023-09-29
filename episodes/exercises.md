---
title: Designing Assessments
teaching: 25
exercises: 70
start: yes
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Choose the format for an exercise based on the outcome it is intended to measure.
- Display exercises and their solutions in a lesson site.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- Why are exercises so important in a lesson?
- What are some different types of exercises, and when should they be used?
- How should exercises be presented in a lesson website?

::::::::::::::::::::::::::::::::::::::::::::::::::


## Exercise Your Memory

In a simplified model of memory individuals are equipped with two types of memory:
working (also called short-term) and long-term.
Long-term memory essentially has unlimited storage but is slow to access, whereas
working memory is quicker to access but can only hold a limited number of items at a time.
For teaching, the goal is to help learners move the new things they've learned from
working memory into long-term memory.
One of the ways lesson developers can aid in this process is through exercises.
In addition to providing formative assessments for instructors and check for misconceptions and broken
mental models, exercises help move new skills and concepts into long-term memory by providing learners an opportunity to practice what was recently learned.
Exercises should occur frequently throughout the lesson because they move items
to long-term memory and free up learners' working memory for new items.

Creating exercises builds upon the learning objectives you created earlier in the lesson design process.
You can design exercises based on the actions/skills you described in your
learning objectives (the learning outcomes you intend for the lesson).
This will be easier if your wrote learning objectives with specific action verbs.
Specific verbs can help you decide what action you want the learners to perform in the exercise.
E.g. actions such as "explain" and "describe" may be better assessed by discussions
and multiple choice questions, while "solve," "construct," "test" and other
higher-level cognitive skills may be better assessed by debugging tasks, [code-and-run][code-and-run],
or use-in-a-different-context exercises.

::: callout

### Resources to Explore for More Example Assessment Types

  - [Exercise Types Chapter from Teaching Tech Together](https://teachtogether.tech/en/index.html#s:exercises)
  - [Edutopia's 56 Examples of Formative Assessment](https://www.edutopia.org/groups/assessment/250941)
  - [H5P Examples and Downloads for Interactive Content](https://h5p.org/content-types-and-applications)

:::



::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Exercise Types and When to Use Them (15 minutes)

The Trainers will assign you to pairs or small groups,
and give each group an exercise type to focus on.
Each group should assign a notetaker,
to summarise your discussion at the end of the exercise.

Read about your given exercise type
[in the *Exercise Types* chapter of *Teaching Tech Together*](https://teachtogether.tech/en/index.html#s:exercises) by following the relevant link below.

- [fill-in-the-blanks][blanks]
- [faded examples][faded-ex]
- [Parsons problems][parsons]
- [minimal fix][minimal]

Then, discuss the following questions together:

- What kind of skills would an exercise of this type assess?
  Try to identify some action verbs like those we used to write lesson objectives earlier in the workshop.
- Would this type of exercise be suited to a novice audience?
  Or is it a better fit for intermediate or advanced learners?
- Would this kind of exercise work well in an in-person workshop setting?
  Would it be better suited to self-directed learning and/or a virtual workshop?

Share the major points of your discussion in the collaborative notes document.


::::::::::::::::::::::::::::::::::::::::::::::::::


As you discussed with your group in the last exercise,
different types of learning objectives work better for novices,
while others are a better fit for competent practitioners or experts.

This can be understood in terms of the types of exercises that suit the objective:
exercise types that help manage cognitive load for the learner,
such as [fill-in-the-blanks][blanks], [faded examples][faded-ex] or [Parsons problems][parsons]
(which all provide a lot of the guiding process/scaffolding code and allow the learner to focus on a specific concept or skill)
are a good fit for a novice, to whom all elements of the topic are new.
However, these kinds of exercise do not provide an opportunity for learners
to develop higher-level skills,
such as the ability to create whole new functions or scripts,
or to extrapolate from the examples they have seen to solve a different kind of problem.
Indeed, example and exercise types that are helpful to novices 
may even be counter-productive for learners with a greater level of expertise[^1].

Thus you want to choose your objectives to fit your intended audience and your exercise formats to fit your objectives.


::::::::::::::::::::::::::::::::::::  testimonial

*"Different types of lesson objectives (LOs) are better fit for novices,
while others are better fit for competent practitioners, etc. and
if exercises (formative assessments) are well aligned to LOs,
[they] will automatically serve the corresponding audience.
Thinking in terms of LOs
(What should a learner do in order to achieve this specific LO?
Is this LO exactly what learners are expected to achieve by the end of this piece of instruction? etc.)
is easier than thinking in terms of LOs + audience + content.
LOs should be tailored to the audience, and,
if this is well done, you may stop worrying about the audience.
Create LOs for the specific audience and create assessments for specific LOs."*

\- Dr. Allegra Via, Carpentries Instructor Trainer


::::::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Assessing an Objective (30 minutes)

Using one of the exercise formats you have learned about so far,
design an exercise that will require learners to perform one of the actions
described in the objectives you wrote earlier,
and that assesses their ability to do so.

These should be assessments of the lower-level objectives defined
for individual episodes in the lesson,
as opposed to the lesson-level objectives you wrote first.

Trainees working as a team can choose whether to 
work together on discussing and designing a single exercise to assess a single objective,
or to divide their efforts and each focus on an exercise for their own episode.
If you choose to take the latter approach and finish with time to spare,
spend the remainder reviewing and providing feedback on one another's assessments.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::: callout

## Assessing Knowledge Before a Workshop

The same approach to designing exercises within a lesson can also be used
to create a short "re-assessment" questionnaire for potential learners
to complete when they register for a workshop teaching the lesson
(or for self-evaluation before following the lesson on their own).
You can use [the list of prerequisite knowledge that you defined earlier](audience.md#defining-prerequisite-knowledge)
to help with this.

If you collect the results of this questionnaire,
use it to follow up with people who have registered for the workshop
but do not fit the intended target audience,
to manage their expectations about how useful the workshop will be for them.

::::::::::::::::::::::::::::::::::::::::::::::::::


## Demo of Writing an Exercise

Well-designed exercises are one of the most valuable resources for an instructor and
any time spent on this is well invested.


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
format the MCQ you designed previously as an exercise in your lesson site.


::::::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: More Practice with Fenced Divs (10 minutes)

Return to the bulleted list of prerequisite knowledge or skills you added to the `index.md` file of your lesson and
use fenced divs to display it in a formatted box with the `prereq` class.
Note that all lesson objectives in fenced divs will be combined into
one box at the top of each episode.


::::::::::::::::::::::::::::::::::::::::::::::::::



[blanks]: https://teachtogether.tech/en/index.html#fill-in-the-blanks
[code-and-run]: https://teachtogether.tech/en/index.html#code-run
[faded-ex]: https://teachtogether.tech/en/index.html#faded-examples
[parsons]: https://teachtogether.tech/en/index.html#parsons-problem
[minimal]: https://teachtogether.tech/en/index.html#minimal-fix


:::::::::::::::::::::::::::::::::::::::: keypoints

- Exercises are important for learners to move what they've learned to long-term memory.
- Some types of exercises are better for particular audiences and to address certain objectives.
- Exercises (and solutions) go in blocks using fenced divs in the lesson.

::::::::::::::::::::::::::::::::::::::::::::::::::


[^1]: [Kirschner et al. 2006](learners/reference.md#litref)
