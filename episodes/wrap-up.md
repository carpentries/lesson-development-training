---
title: Wrap-up
teaching: 15
exercises: 10
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Summarise the lesson development process introduced in this training.
- Identify next steps to take that will ensure further progress towards a completed, thoroughly tested lesson.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What steps will you take after this training?
- How could this training be improved?

::::::::::::::::::::::::::::::::::::::::::::::::::

We have reached the end of this training.
Throughout this training we promoted an iterative, collaborative approach to lesson development (as many other initiatives in The Carpentries community are conducted). 
The iterative approach ensures that you regularly receive feedback that will help you adjust and refine the design and content of your lesson.
Collaboration helps bring different skills and perspectives to a project and share the load of the work required to bring the project successfully past the finishing line. 
For lesson projects, this shared effort also extends to maintaining and updating the lesson after the initial development phase.

## Next steps
Here are some suggestions for what to do next, to make sure that you finish drafting your lesson, test it out, and eventually bring it to a stable state.

### Complete your Lesson Developer certification!
The [checkout process](../learners/checkout.md) is designed to help you complete the first cycle through [the iterative backward design process](lesson-design.md), giving you an opportunity to deliver some lesson content, gather feedback, and use that information to evaluate how effective your lesson is in teaching what you want learners to learn.
In addition to making you a certified Lesson Developer, Checkout will help you identify what could be improved in your lesson and help you plan the next iteration of development.

### Learn more skills for effective collaboration
Trainees with less experience working in GitHub will benefit from joining a GitHub Skill-up session after this training.
The skill-up teaches good practices and features of the GitHub interface that will help you manage tasks, review contributions, and work together more effectively.

### Learn more about best practices in lesson design
Explore the [literature references](../learners/reference.md#literature-reference-litref) for this curriculum for greater insight into the principles underpinning what you learned in the training.
The training has given you a strong foundation but there is a lot more to be learned about effetive curriculum design and these resources are a great place to start.

### Identify oustanding tasks
This training covers a lot of concepts and leads you through many different tasks in a limited amount of time.
To help you prioritise what to work on next, consider the following prompts and make notes of your answers.

- Which of the exercises set so far in this training did you not have time to complete?
- What do you still need to add/work on?
- What can you remove/consider removing?
- How will the narrative and example data you have chosen for your lesson support teaching and assessment?
- What diagram or other visual aids could you create/add to supplement your text?

### Organise your knowledge
Take some time to think back on what has been covered so far,
then make some notes on the most important points and actions you want to take away from that.
The Trainers and other participants will not look at this - it is only for you.

If you do not know where to start, consider the following list for a starting point:

- draw a concept map, connecting the material
- draw pictures or a comic depicting one or more of the concepts
- write an outline of the topics we covered
- write a paragraph or “journal” entry about your experience of the training today
- write down one thing that struck you the most

### Assess your lesson design
_(This exercise adapted from [Via et al. 2020](learners/reference.md).)_

When the first draft of your lesson content is nearly complete, consider mapping out the relationships between the objectives of your episode and the examples and exercises via which they will be taught and assessed.
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

### Add your design notes to the lesson site
Consider adding the Design Notes you have been working on as a page on your lesson site, to provide context for furture discussions of the intended target audience and scope of the lesson.

1. Replace the first 13 lines of your Design Notes document with

  ```
  ---
  title: Lesson Design Notes
  ---
  ```
2. Save the file to the `instructors/` directory, and any images used in the file to the `episodes/fig` directory.
   Adjust the paths to source files for images to begin `episodes/fig/`.
3. Add the filename below `instructors:` in `config.yml` as you did 
   [for episode filenames below `episodes:` previously](./infrastructure.html#adding-a-new-episode-to-the-lesson-navigation).
   For example, if your file is saved with the name 'design-notes.md':

  ```yaml
  # Information for Instructors
  instructors:
  - design-notes.md
  ```

This will make the page accessible from the 'More' dropdown in Instructor View.

_Note that concept maps with GraphViz are not currently supported by the lesson infrastructure,
so any concept maps added to the document on CodiMD will not be displayed correctly on the lesson site._


## Feedback
The Trainer(s) will ask for feedback on the training.
Take some time to provide this feedback, before moving onto the second part of this task.

:::::::::::::::::::::::::::::::::::::::: challenge

## One Up, One Down (10 min)
Provide one up, one down feedback on Collaborative Lesson Development Training.

- Say only one thing, and try not to repeat points others have already raised.
  This gets harder for those who come later!
- Trainers should try not to respond, only record responses (e.g. in the CodiMD).
  This is also hard, but important!

::::::::::::::::::::::::::::::::::::::::::::::::::

Good luck and keep in touch as you continue to develop and refine your lesson!

:::::::::::::::::::::::::::::::::::::::: keypoints

- Although this training is over, your lesson development journey has only just begun.
- The Carpentries lesson development community offers support with the rest of the process.

::::::::::::::::::::::::::::::::::::::::::::::::::
