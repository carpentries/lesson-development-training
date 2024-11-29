---
title: How to Write a Lesson
teaching: 30
exercises: 40
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Estimate the time required to teach a lesson.
- Summarise the content of a lesson as a set of questions and key points.
- Connect the examples and exercises in a lesson with its learning objectives.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- Why do we write explanatory content last?
- How can I avoid demotivating learners?
- How can I prioritise what to keep and what to cut when a lesson is too long?

::::::::::::::::::::::::::::::::::::::::::::::::::

![
Now that we have designed assessments to measure attainment of the objectives set for the lesson,
it is time to begin developing teaching content to give learners the knowledge and skills
they need to succeed in those assessments.
](./fig/cldt-step-3.svg){
alt="An overview of the iterative process of lesson design and development,
adapted from Nicholls' five phases,
with step 3, 'Develop relevant content' highlighted."
width="67%"
}

## Writing Explanatory Text

Explanatory text (including examples) help connect your exercises together into a cohesive lesson.
If your exercises are train stations and scenic views,
the explanatory text is the train tracks that connect them.
Often times the examples and exercises may seem like a good draft for you to teach.
However, the explanatory text makes it possible for other instructors and self-directed learners
to follow along by providing all the relevant information directly in the lesson.
It can also help you remember your goals and stay on track teaching.

How much text to include is often a question of personal style while balancing the needs of
potential users, both other instructors and learners.
You want to find the balance between providing enough information for learners to meet the learning objectives
without increasing cognitive load with extraneous information.
In this section we will discuss factors to consider when you are writing explanatory text.

There are trade-offs to consider when preparing a site for use as an instructional guide vs use as a self-directed learning resource.
Typically, self-directed learning resources are more verbose where instructional guides are aimed at an audience that can fill in the gaps on their own.
However, very sparse text is less likely to be re-usable by other instructors as instructors
may have different skill levels with the lesson content or differing mental models.
In general, it is not a good idea to assume others, learners or instructors,
will know what you were thinking when you wrote the content
so, if in doubt, be explicit.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Examples Before Exercises (20 minutes)

Looking back at one of the exercises you designed before:
what examples could you include in your narrative to teach learners the skills
they will need to apply to complete the formative assessments you have designed?

Outline one of these examples in your lesson design notes.

::::::::::::::::::::: hint 

### Examples

In the Software Carpentry Plotting and Programming with Python Lesson there is an exercise to load and inspect CSV file for Americas.
In the lesson, before the exercise, the Instructor demonstrates an example of how to load the data table for another continent (Oceania)
and explores the values with a few different functions.
This shows learners how to call the function to load the CSV into a data frame,
and demonstrates what success looks like for their exercise.

In the Python Interactive Data Visualization Lesson in the Incubator, there is an exercise to find the correct widget (a slider) 
for an action and modify the script to use it.
In the lesson, before the exercise, the instructor introduces a cheatsheet and documentation for interactive widgets and
then creates a dropdown widget for the application.
The slider widget required in the exercise has not been demonstrated but
the preceding example shows all of the necessary steps to add a widget,
and provides the supporting information that learners can consult to discover
how to implement the specific tool.

::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::


## Less is More

Trying to fit too much content into a lesson is counter-productive.
It is better to cover less and provide a smaller but stable foundation for learners to build upon.

You should also consider a realistic workshop length for teaching your lesson.
It is difficult to keep learners attentive for many hours over many days.
Most Carpentries workshops are two work days of lesson material as it is difficult for learners to
attend 4 full days of a workshop.
Although, there are some in the community who will run workshops that are three days to cover additional material.

As you consider the length of your lesson discuss with your collaborators and ask yourself:

- What is essential to include?
- What can be left out if needed?
- Are there checkpoints where the lesson could end if needed?
- Can important concepts be moved up earlier to ensure they are covered?

In the end, the only way to know for sure is to teach the lesson, measuring how long it takes to teach.
Borrowing from television, The Carpentries community calls these early workshops, pilot workshops.
As you run pilot workshops, you can note the length of time spent in each episode.
You might find the [template for notes on pilot workshops][pilot-notes-template] helpful as it includes a table for episode and exercise timings.
Instructors commonly report running short on time in workshops.
Thus, it is better to assume that you are under-estimating rather than over-estimating the length.
It is better to have additional time for discussion, review, and wrap-up than to rush through material to fit it into the remaining time.

If, after piloting your new lesson, you find that you did not have time to cover all the
content, approach cutting down the lesson by identifying which learning objectives to
remove. Then take out the objective(s) and the corresponding assessment(s) and explanatory
content. You may consider making a [concept map][mental-map-instructor-training] to help identify which objectives depend on one another.

Alternatively, if you decide to keep certain objectives in the lesson, you can add
suggestions on which objectives can be skipped to the Instructor Notes for the lesson.
Instructor Notes are meant to convey teaching tips and advice to other instructors teaching your 
lesson and will be discussed in more detail later on in section ["Preparing to Teach"](preparing.md).

As you add notes and think about what to cut, remember, reducing the number of lesson
objectives can help with managing learner (and instructor) cognitive load.


::::::::::::::::::::::::::::::::::::  testimonial

*"the five ways to handle an extraneous overload situation are to:*

- *eliminate extraneous material (coherence principle),*
- *insert signals emphasizing the essential material (signaling principle),*
- *eliminate redundant printed text (redundancy principle),*
- *place printed text next to corresponding parts of graphics (spatial contiguity principle), and*
- *eliminate the need to hold essential material in working memory for long periods of time (temporal contiguity principle)."*

\- [Renkl (2014)](learners/reference.md#litref)


::::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::  discussion

## Lesson Time Management (10 minutes)

(5 minutes) In the shared notes document,
note down your answers to these questions:

- From a design perspective, at what point is a lesson too long?
- What factors influence and constrain the length of a lesson?
- How might you prioritise what to keep if you have to cut lesson content down?

(5 minutes) In the remaining time,
your Trainers will lead a discussion based on the responses.

::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

## Trainer Note

To get started on the discussion part,
try reading out an interesting response and asking for more detail from the trainee who wrote it.
Ask one of the other trainers/helpers to take notes of this discussion in the collaborative
note-taking document.

This is a good opportunity to remind trainees about
how counter-productive it can be to try to cover more content than the time allows.
(See [the earlier section on lesson scope](./objectives.md#lesson-scope).)

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

## Other Important Considerations for Lesson Content

### Language 

When writing your lesson text you also want to avoid unintentionally demotivating your learners.
Make time to review your text for:

- [dismissive language][dismissive-language-instructor-training] - e.g. 'simply', 'just'
- use of [stereotypes][stereotype-threat-instructor-training] (check learner profiles for stereotypes too)
- [expert awareness gaps][expert-awareness-gap-instructor-training], i.e. places where you may be assuming the learners know more than they actually do
- use of different terms or notations with the same meaning interchangeably without explanation, e.g. using the terms "shell", "bash", "terminal" and "console" to describe the command line interface, or "variables" and "columns" for column headings in data tables
- unexplained or unnecessary jargon/terminology (as your learners may come from different backgrounds, may be novices, not native English speakers, and a term in one domain/topic may mean something else entirely in another)
- unexplained assumptions
- sudden jumps in difficulty/complexity

### Accessibility

You should also review your text thinking about accessibility.
This includes:

  - Avoiding regional/cultural references and idioms that will not translate across borders/cultures
  - Avoiding contractions i.e. don't, can't, won't etc.
  - Checking that all figures/images have well written alternative text, including [writing alternative text for data visualizations](https://medium.com/nightingale/writing-alt-text-for-data-visualization-2a218ef43f81). An alternative text contains an invisible description of an image which is read aloud to blind users by screen readers providing alternative text-based format for images. See [the Workbench documentation for directions on how to add alternative text and captions to images in a lesson](https://carpentries.github.io/sandpaper-docs/episodes.html#figures)
  - Checking the header hierarchy - no h1 headers in the lesson body, no skipped levels
  - [Using descriptive link text](https://www.imperial.ac.uk/staff/tools-and-reference/web-guide/training-and-events/materials/accessibility/links/) - no "click here" or "this page", etc.
  - [Checking the text and foreground contrast for images](https://contrastchecker.com/)

::::::::::::::::::::::::::::::::::::::  challenge

## Optional Exercise: Alternative Text for Images (5 minutes)

Which of the following is a good alt-text option for the image below?

![Atmospheric Carbon Dioxide at Mauna Loa Observatory](https://gml.noaa.gov/webdata/ccgg/trends/co2_data_mlo.png){alt="Line graph of increasing carbon dioxide at the Mauna Loa Observatory from 1958 to present"}

1. Graph of data
2. Graph with increasing lines
2. Line graph of increasing carbon dioxide in ppm at the Mauna Loa Observatory from 1958 to present
3. Line graph of increasing carbon dioxide in ppm at the Mauna Loa Observatory, Hawaii, United States, from 1959 to present including values from each year. Red line shows variation in each year and black line is average for each year. 1959 = 315.90 ppm, 1960 = 316.91, 1961 = 317.64 ...

[_Data/Image provided by NOAA Global Monitoring Laboratory, Boulder, Colorado, USA_](https://esrl.noaa.gov/)

:::::::::::::::::::  solution

The third option, "Line graph of increasing carbon dioxide in ppm at the Mauna Loa
Observatory from 1958 to present", is the best option. It describes the type of plot,
what is measured, and the trend.

The first two options are too vague. They mention a graph but don't give enough
info to know what the graph is actually showing.

The last option is overly descriptive and starts to list the data itself.
It is better to include a shorter, but informative, description and a link to the
data instead.

:::::::::::::::::::::::::::::

:::::::::::::::::::::::: instructor

May want to point out that the answers in the current version of this exercise do not
have diagnostic power.

:::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

### Glossary of Terms

When writing a lesson, you should also consider adding key terms or jargon to the lesson glossary
for the lesson. 
In your shared notes document, you can start such a glossary as you develop your lesson, to 
keep a record of the terminology your audience needs to be familiar with.

Many of these terms may also be useful for other lessons and can be added to [Glosario][glosario], a multilingual glossary for computing and data science terms.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Explain Your Terminology (5 minutes)

In your shared notes document, add a list of terms or jargon from your lesson, 
along with their definitions. 

You do not have to have a complete list now, but it is good to start working on it - you can always
come back and update it later.

::::::::::::::::::::::::::::::::::::::::::::::::::

### Questions and Keypoints

In addition to objectives, a [completed episode also requires](https://carpentries.github.io/sandpaper-docs/episodes.html?#required-elements)
questions the episode answers and the keypoints a lesson covers.

The questions helps learners understand what to expect from a lesson as they might
not yet understand the learning objectives.

The keypoints wrap up the lesson by providing answers to each of the questions.
Keypoints also help self-directed learners review what they learned, remind instructors to
recap what was covered in an episode, and help you ensure you answered all the questions
you intended for an episode.


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Completing episode metadata (10 minutes)

In your shared notes document, add key points and questions for your episode.

::::::::::::::::::::::::::::::::::::::::::::::::::

## Polishing a lesson

Lessons do not need to be perfected prior to teaching them the first time.
In fact, keeping things relatively basic leaves you some flexibility while you run through the first few iterations
of teaching the lesson, collecting feedback, and using that to guide improvements.

However, once you find that the lesson is beginning to reach something like a stable state,
you may find [the checklist for lesson reviewers in The Carpentries Lab][lab-reviewer-checklist]
useful as a guide for polishing the design and content.
The checklist describes criteria for a lesson to meet a high standard in terms of its
accessibility, design, content, and supporting information.


[dismissive-language-instructor-training]: https://carpentries.github.io/instructor-training/04-expertise.html#just-and-other-dismissive-language
[instructor-notes]: https://carpentries.github.io/workbench/transition-guide.html#instructor-notes
[lab-reviewer-checklist]: https://github.com/carpentries-lab/reviews/blob/main/docs/reviewer_guide.md#reviewer-checklist
[mental-map-instructor-training]: https://carpentries.github.io/instructor-training/02-practice-learning.html#mapping-a-mental-model
[stereotype-threat-instructor-training]: https://carpentries.github.io/instructor-training/09-eia.html#stereotypes
[sandpaper-docs-learners]: https://carpentries.github.io/sandpaper-docs/editing.html#learners

:::::::::::::::::::::::::::::::::::::::: keypoints

- The objectives and assessments provide a good outline for an episode and then the text fills in the gaps to support anyone learning or teaching from the lesson.
- It is important to review your lesson for demotivating language, cognitive load, and accessibility.
- To reduce cognitive load and ensure there is enough time for for the materials, consider which lesson objectives are not needed and remove related content and assessments.

::::::::::::::::::::::::::::::::::::::::::::::::::
