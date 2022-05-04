---
title: Designing assessments
teaching: 25
exercises: 70
start: yes
---

::::::::::::::::::::::::::::::::::::::: objectives

- Choose the format for an exercise based on the outcome it is intended to measure.
- Display exercises and their solutions in a lesson site.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- Why are exercises so important in a lesson?
- What are some different types of exercises, and when should they be used?
- How should exercises be presented in a lesson website?

::::::::::::::::::::::::::::::::::::::::::::::::::


## Exercise Your Memory

A simple model of memory is that individuals have two types of memory, 
working (also called short-term) and long-term.
Long-term memory is essentially unlimited storage but slow to access whereas
working memory is quicker to access but can only hold a limited number of items at a time.
For instructors, the goal is to help learners move the new things they've learned from 
working memory into long-term memory.
One of the ways lesson developers can aid in this process is through exercises.
In addition to providing formative assessments for instructors, exercises help move 
new skills and concepts into long-term memory by providing learners an opportunity 
to practice what was recently learned.
Exercises should occur regularly throughout the lesson because they move items 
to long-term memory and free up learners' working memory for new items.


Creating exercises builds upon the learning objectives you created earlier in the lesson design process.
You can design exercises based on the actions/skills you described in your 
learning objectives (the learning outcomes you intend for the lesson).
You can benefit here from creating learning objectives with specific action verbs.
Specific verbs can help you decide what action you want the learners to perform in the exercise.
E.g. actions such as "explain" and "describe" may be better assessed by discussions 
and multiple choice questions, while "solve," "construct," "test" and other 
higher-level cognitive skills may be better assessed by debugging tasks, code-and-run, 
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
For example, novices benefit significantly from worked examples (fully solved example problems)
as it reduces their cognitive load 
and worked examples are not as helpful in building skill for individuals with more expertise as they have to match up the information given with their mental model which can increase the cognitive load [Kirschner, 2006](https://github.com/carpentries/instructor-training/blob/gh-pages/files/papers/kirschner-minimal-guidance-fails-2006.pdf) <!--- Maybe this should reference Kalyuga et al 2001 and 2003 instead or in addition? Or the review  of expertise reversal effect - https://doi.org/10.1007/s10648-007-9054-3.  Also might have brought up worked example too soon as it is in the next section of notes -->
Thus you want to choose your objectives to fit your intended audience and your exercise formats to fit your objectives.


::::::::::::::::::::::::::::::::::::  testimonial

*"Different types of LOs are better fit for novices,
while others are better fit for competent practitioners, etc and
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

<!--- I'm not sure how to work in this part of the outline now..

The worked example effect -
worked examples are more effective than problem-solving for novices,
less effective (even counter-productive) for competent practitioners.
Allegra: worked examples cannot be used to achieve high Bloom's levels of cognitive complexity
(critical thinking/problem solving),
that's why they are not effective for competent practitioners.
If you create exercises suitable for low Bloom's level LOs,
they will be effective for novices but NOT for competent practitioners.
-->

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Assessing an Objective (30 minutes)

Using one of the exercise formats you have learned about so far,
design an exercise that will require learners to perform one of the actions
described in the objectives you wrote for your lesson,
and that assesses their ability to do so.


::::::::::::::::::::::::::::::::::::::::::::::::::

## Demo of Writing an Exercise 

Well-designed exercises are one of the most valuable resources for an instructor and 
any time spent on this is well invested.

<!--- will there be an example lesson that the trainer is working on ? -->

To create an exercise in the Carpentries Workbench, 
you can use colon-delimited sections called 'fenced divs'.
In fact there are many types of boxes in the lesson infrastucture, called "special blockquotes", 
that use fenced divs.
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

Some other types of formative assessment include:

- **Think, pair, share** - Learners _think_ about an answer to a question, _pair_ up
with a classmate to discuss their answer, and then _share_ out the consensus they came to 
with the class.
- **Sticky notes and written feedback** - Learners each get two colors of sticky notes. 
If they fall behind or run into an issue, they can put up the 
color that signals they need help.
If they have completed and exercise or think the instructor could speed up, they put their
other sticky note up.
Then at breaks these stickies can turn into written feedback "minute cards", where the learner 
writes down one thing they were confused about or that could be improved and one thing that went well
or they really liked learning.
- **Reflective assessment** - Learners spend time reflecting on what they have learned so far.
This can be really helpful for "metacognition", where learners think about the process of learning themselves.



::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: More Practice with Special Blockquotes (10 minutes)

Return to the bulleted list of lesson objectives you added to the `index.md` file of your lesson and
use special blockquotes to display it in a formatted box with the `.prereq` class.


::::::::::::::::::::::::::::::::::::::::::::::::::



[blanks]: https://teachtogether.tech/en/index.html#fill-in-the-blanks
[parsons]: https://teachtogether.tech/en/index.html#parsons-problem
[minimal]: https://teachtogether.tech/en/index.html#minimal-fix


:::::::::::::::::::::::::::::::::::::::: keypoints

- Exercises are important for learners to move what they've learned to long-term memory.
- Some types of exercises are better for particular audiences and to address certain objectives.
- Exercises(and solutions) go in special challenge blockquotes using fenced divs in the lesson.

::::::::::::::::::::::::::::::::::::::::::::::::::


