---
title: Part 1 Wrap-up
teaching: 5
exercises: 25
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Summarise the lesson development process introduced in this training.
- Describe the trial run task to be completed before the next part of the training
- Identify remaining tasks that should be completed before trialling lesson content.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What have we learned so far?
- What needs to be done before the next part of the training?

::::::::::::::::::::::::::::::::::::::::::::::::::

Recent sections of this training have focused on how to design effective
assessments and write a lesson that will be engaging and motivating for learners.
We provided further opportunities to apply these concepts to the development
of a lesson website with The Carpentries Workbench.
Next, we explored The Carpentries lesson development ecosystem and how a new lesson
project can fit into that.
We finished up with a discussion of the importance of teaching a new lesson
and how best to prepare for that experience.

The final sessions will focus on collaboration skills, exploring how trainees can
curate their repository and manage their project to foster collaboration and
build community around a lesson.

Before that, there will be an extended break during which trainees should conduct a
_trial run_ of the lesson content they have been developing in the workshop so far.
When the training recommences,
there will be an opportunity for trainees to share their experiences and reflections
from those trial runs, and to discuss what impact that will have on the next stages
of their lesson development.

:::::::::::::::::::::::::::::::::::::::  challenge

## Polish a Lesson (20 minutes)

This exercise provides you with a chance to look back over 
everything you have sketched out for your episode(s) and the lesson as a whole 
and consider what still needs to be done before it can be taught.

You can use this time however you judge will be most beneficial
to your preparations for teaching your episode in a trial run.

If you are not sure how to start, consider the following prompts:

- Which of the exercises set so far in this training did you not have time to complete?
- What do you still need to add/work on?
- What can you remove/consider removing?
- How will the narrative and example data you have chosen for your lesson support teaching and assessment?
- What diagram or other visual aids could you create/add to supplement your text?


::::::::::::::::::::::::::::::::::::::::::::::::::


Please spend some time reflecting on what you learned so far and then provide another round of feedback 
to your trainers.

::: challenge

## Organise Your Knowledge (10-15 min)

Take some time to think back on what has been covered so far,
then make some notes on the most important points and actions you want to take away from that.
The Trainers and other participants will not look at this - it is only for you.

If you do not know where to start, consider the following list for a starting point:

- draw a concept map, connecting the material
- draw pictures or a comic depicting one or more of the concepts
- write an outline of the topics we covered
- write a paragraph or “journal” entry about your experience of the training today
- write down one thing that struck you the most

:::::::::::::

::::::::::::::::::::::::::::::::::::::: challenge

### Optional Homework: Assessing Your Lesson Design

(This exercise adapted from [Via et al. 2020](learners/reference.md).)

When the first draft of your lesson content is nearly complete,
consider mapping out the relationships between the objectives of your episode 
and the examples and exercises via which they will be taught and assessed.
For example,

> The read CSV and inspect demo supports Objective 2 
> (load a simple CSV data set with Pandas) 
> and will be delivered using participatory live coding.
> The objective will be assessed with an exercise that 
> requires learners to apply the read_csv function to another file
> and count the rows in the resulting DataFrame object.

- Does any of your planned content not support any learning objectives?
- Is there at least one piece of content planned for each learning objective?
- Is there a formative assessment planned for each learning objective?

:::::::::::::::::::::::::::::::::::::::::::::::::


::: challenge

## Feedback (5 min)

The Trainer(s) will ask for feedback on the training so far.
Take some time to provide this feedback, before moving onto the second part of this task.

:::::::::::::

Please stay in touch as you plan for your trial run.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

## Adding Design Notes to the Lesson Site

If trainees would like to add the Design Notes document
they have been working on to their lesson site,
they can do the following:

1. replace the first 13 lines with

  ```
  ---
  title: Lesson Design Notes
  ---
  ```
2. save the file to the `instructors/` directory, and any images used in the file to the `episodes/fig` directory
   (the paths to source files for images will need to be adjusted to begin `episodes/fig/`)
3. add the filename below `instructors:` in `config.yml` as they have done 
   [for episode filenames below `episodes:` previously](./infrastructure.html#adding-a-new-episode-to-the-lesson-navigation).
   For example, if their file is saved with the name 'design-notes.md':

  ```yaml
  # Information for Instructors
  instructors:
  - design-notes.md
  ```

This will make the page accessible from the 'More' dropdown in Instructor View.

_Note that concept maps with GraphViz are not currently supported by the lesson infrastructure,
so any concept maps added to the document on CodiMD will not be displayed correctly on the lesson site._

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: keypoints

- We have learned about the importance of exercises and data in a lesson, the ecosystem The Carpentries provides for lesson development, and how to prepare to teach a lesson for the first time.
- Before the next part of the training, you should teach a part of your new lesson to a real audience and reflect on the experience.

::::::::::::::::::::::::::::::::::::::::::::::::::
