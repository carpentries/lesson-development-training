---
title: Example Data and Narrative
teaching: 15
exercises: 50
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Find candidate datasets to use in a lesson.
- Evaluate the suitability of a dataset to be used in a lesson.
- Choose examples that will prepare learners for formative assessments in the lesson.
- Develop a story

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- Why should a lesson tell a story?
- What considerations are there when choosing an example dataset for a lesson?
- Where can I find openly-licensed, published data to use in a lesson?

::::::::::::::::::::::::::::::::::::::::::::::::::

![
Now that we have designed assessments to measure attainment of the objectives set for the lesson,
it is time to begin developing teaching content to give learners the knowledge and skills
they need to succeed in those assessments.
](./fig/cldt-step-3.svg){
alt="An overview of the iterative process of lesson design and development, 
adapted from Nicholl's five phases,
with step 3, 'Develop relevant content' highlighted."
width="67%"
}

## Creating a Narrative

<!--- Should this section go before LO and questions? -->

Writing your lesson as a story helps learners stay motivated and engaged.
The story you create can also help learners more easily connect how the skills they
are learning now could be useful after the workshop.
You can enable learners to make connections between what they learn in your lesson and their
own work by creating a narrative that resembles a situation the learners might
encounter there.

You may find that images and figures enhance your narrative.
Images are powerful communicators, conveying a lot of information with few or no words.
Images can also be distracting for learners.
If you choose to include images as part of the narrative of your lesson,
be sure that they are consistent with the situation you are describing
so that they do not increase learners' cognitive load.

Depending on the tool you are teaching, you might also include a particular dataset as a part of the story you are weaving into your lesson.
It is common for lessons to include a dataset that is used in examples and discussed throughout.
This can help you maintain a narrative flow and make the lesson feel more authentic.
Even if your topic doesn't require a dataset, deciding on a consistent narrative will
help create a flow between episodes and reduce cognitive load for learners.

:::::::::::::::::::::::::::::::::::::::::: callout

## Varying Examples

> _Use varied examples if you want to teach abstract concepts._
> 
> -- Neil Brown
> 
> From [_How Your Mind Learns to Program_](https://neverworkintheory.org/2022/05/25/brown-mind-learns.html), a lightning talk in the _Never Work In Theory_ series

The focus of this episode is on finding 
one central example to be used throughout a lesson.
However, where you wish for learners to develop understanding of more abstract concepts,
you should try to provide a variety of examples with a common theme.
This could be achieved by providing multiple opportunities 
to recognise and apply the concept in taught examples, activities, and exercises.

::::::::::::::::::::::::::::::::::::::::::::::::::

## Finding Images

Copying an image from a website is technologically simple but can be legally and ethically complex.
Images are intellectual property and are subject to intellectual property laws
including, but not limited to, copyright and trademark laws.
These laws differ by country but are consistent in theme:
do not take intellectual property that does not belong to you without permission.

When looking for images that illustrate the narrative of your lesson,
avoid copying images that do not include a reuse license.
Assume that you cannot reuse these images unless you seek written permission from the image creator or owner.
Instead, look for images that indicate that they are in the public domain
or carry a permissive reuse license such as CC0 or CC-BY.
Public domain images can be freely reused and adapted.
Images carrying a reuse license can be used and adapted in accordance with their license terms.

If you cannot find reusable images that match your narrative, you can
create your own images or seek help from others in the Carpentries community.
When incorporating original images into your lesson, be sure to license these images
to be compatible with the license on the rest of your lesson materials.

The guidance in this section is not a substitute for legal advice.

:::::::::::::::: callout

## Compatible Licenses

Creative Commons offers a chart that identifies which CC licenses are compatible with each other for adaptation ("remix") purposes:
[Creative Commons license comparison chart](https://creativecommons.org/faq/#can-i-combine-material-under-different-creative-commons-licenses-in-my-work).

GNU offers commentary about a variety of licenses for free software; this resource may be valuable when considering a license for code:
[GNU: Various Licenses and Comments about Them](https://www.gnu.org/licenses/license-list.en.html).

::::::::::::::::::

## Finding a Dataset

:::::::::::::::::: testimonial

> It was very distracting to me in a workshop, when we were given a dataset to work with but no-one explained what that data was and what it meant. It prevented me from following what the instructors were actually trying to teach me, while I tried to figure out the meaning of the numbers, columns names etc on my own.

::::::::::::::::::

When searching for a dataset to use in your lesson,
there are a number of factors to consider.
First, if possible you want the dataset to be an authentic use
case for researchers in your target audience.
This means balancing the size and complexity of a dataset
while avoiding additional cognative load for learners.
The dataset may need a certain number of observations
to demonstrate some of the skills you are teaching or have a
number of variables that is sufficiently similar to what learners may encounter
in their work to feel authentic.
At the same time, you want your learners to be able to interpret the
data fairly easily during the lesson so they can focus on the skills
you are teaching.
This may mean you will need to subset your dataset by removing some observations (rows) or variables
observed (columns).

You may also want to include and review a data dictionary in your lesson,
explicitly taking the time to review the information included in the
dataset.
For inspiration, see the [Social Sciences Data Carpentry data dictionary](https://datacarpentry.org/socialsci-workshop/data/).
An additional factor to consider when choosing a dataset to include is
the license.
You want to find a dataset where the data provider allows for you to freely use it.
The best option is a dataset with a CC0 (Public Domain Dedication) license, as
other licenses may have more ambiguity around data reuse.
Lessons included in [The Carpentries Incubator][carpentries-incubator] are encouraged to use CC0 licensed data, and may be required to do so to qualify for peer review in [The Carpentries Lab][carpentries-lab].
Even with a CC0 license, you will still want to follow best practice in
giving attribution to the data provider or collecting agency.

:::::::::::::::: callout

## More CC0 License Reading

If you'd like to read more about CC0 and CC-BY, Katie Fortney wrote an excellent
[blogpost on why CC-BY is not always a good fit](https://osc.universityofcalifornia.edu/2016/09/cc-by-and-data-not-always-a-good-fit/).

::::::::::::::::::


An example dataset used in the Data Carpentry Ecology lessons is the [Portal
Project Teaching Database](https://figshare.com/articles/dataset/Portal_Project_Teaching_Database/1314459).  This dataset is an actual ecological research project that was simplified for teaching.
The reuse of this dataset throughout the Data Carpentry Ecology lessons helps
stitch together the process of data analysis throughout the workshop, from
data entry and cleaning to analysis and visualization.

When deciding on a dataset, it is also important to consider the ethical use of
each dataset considered. *Does the data contain personally identifiable information?*
*Was the data collected without permission from the groups or individuals included?*
*Will the data be upsetting to learners in the workshop?*
If the answer to any of these questions might be yes, you will need to do more
research on it and continue to look for other options. Commonly data is misused
from historically excluded and exploited groups.
The CARE Principles for Indigenous Data Governance[^1] (Collective Benefit, Authority to Control, Responsibility, and Ethics) are good starting point
for thinking about data sovereignty and considering the ethics of data collected
about an individual or groups of people.

::::::::::::::::::::::::::::::::: instructor

Outline covering the above paragraph - also used in CodiMD template.

### Dataset Considerations

- Ethical use (see prompts below)
- License - CC0 Recommended
- Complexity - Is it easy to understand? Is it sufficiently authentic?
- Number and types of variables

### Questions about Ethical Use of Datasets

- Does the data contain personally identifiable information?
- Was the data collected without permission from the groups or individuals included?
- Will the data be upsetting to learners in the workshop?


::::::::::::::::::::::::::::::



### Examples of Public Repositories

When looking for data to reuse, consider public repositories in the subject area
for your lesson or general data repositories such as:

- [Dryad](https://datadryad.org/)
- [The Data Curation Network's datasets](https://datacurationnetwork.org/datasets/)
- [The Offical Portal for European Data](https://data.europa.eu/)
- [DataONE](https://www.dataone.org/)
- [The Official Portal for Argentina Data](https://www.datos.gob.ar/) (in Spanish)
- [LANFRICA](https://lanfrica.com/)

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Choosing a Dataset or Narrative (30 minutes)

Referring to the advice given above, find an appropriate dataset or a narrative for your lesson.
Identify one or more potential candidates and note down the advantages and disadvantages of each one.

::::::::::::::::::::::::::::::::::::::::::::::::::

People learn faster if they are motivated[^2],
and learners will be motivated if you **teach most useful things first**.
As you think about what story your lesson will tell, it is important to put
the pieces that are most interesting to learners up front.
If they are able to quickly learn tools or skills that they see as useful from your
lesson, they will be more interested in continuing to learn other concepts that are
needed.
You may notice this trend in many of the Software Carpentry lessons. In particular,
many of the coding language lessons (R and Python) have the learners create a plot
very early in the lesson and then go back and teach coding fundamentals such as loops
and conditionals. Visualization of data is often a very motivating and much needed
skill by learners. Getting to visualization early, keeps learners interested in
learning the additional and vital skills where the application might be less clear.

::::::::::::::::::::::::::::::::::::  testimonial

[*"Let them eat cake (first)."*](https://www.youtube.com/watch?v=fQ4t7p6ZXDg)

\- Dr. Mine Çetinkaya-Rundel

::::::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: Examples Before Exercises (20 minutes)

Looking back at one of the exercises you designed before:
what examples could you include in your narrative to teach learners the skills
they will need to apply to complete the formative assessments you have designed?

Examples:
In the Software Carpentry Plotting and Programming with Python Lesson:
Exercise to load and inspect CSV file for Americas ->
In the lesson, the Instructor demonstrates how to load the data table for another continent (Oceania)
and explores the values with a few different functions.
This shows learners how to call the function to load the CSV into a data frame,
and demonstrates what success looks like for this task.
In the Python Interactive Data Visualization Lesson in the Incubator:
Exercise to find the correct widget (a slider) for an action and modify the script to use it ->
In the lesson the instructor introduces a cheatsheet and documentation for interactive widgets and
then creates a dropdown widget for the application.
The slider widget required in the exercise has not been demonstrated but
the preceding example shows all of the necessary steps to add a widget,
and provides the supporting information that learners can consult to discover
how to implement the specific tool.

Outline one of these examples in your episode file.

::::::::::::::::::::::::::::::::::::::::::::::::::



## Summary

Remember, even if you do not need a dataset for your lesson, you should
decide on a narrative.
Centering your lesson around a central example reduces the cognitive load of
switching between examples throughout the lesson.
Using an authentic, yet simple, dataset will also help reduce cognitive
load and help learners to see how they might apply what they learned to their own
projects.
It is also important to consider licensing and ethical considerations when looking
for a lesson dataset.


:::::::::::::::::::::::::::::::::::::::: keypoints

- Using a narrative throughout a lesson helps reduce learner cognitive load
- Choosing a lesson includes considering data license and ethical considerations.
- Openly-licensed datasets can be found in subject area repositories or general data repositories.

::::::::::::::::::::::::::::::::::::::::::::::::::


[^1]: [Carroll et al. (2020)](learners/reference.md#litref)
[^2]: The evidence for this is summarised well in chapter 3,
      _What Factors Motivate Students to Learn?_,
      of [Ambrose et al. 2010](learners/reference.md#litref).
      The Carpentries Instructor Training curriculum also includes
      a helpful summary of 
      [how lesson content can influence Learner motivation](https://carpentries.github.io/instructor-training/08-motivation.html#how-can-content-influence-motivation).

