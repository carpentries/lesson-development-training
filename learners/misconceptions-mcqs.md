---
title: Diagnosing Misconceptions
---
          
Detecting and correcting 
[misconceptions](https://carpentries.github.io/instructor-training/02-practice-learning.html#misconceptions) 
and fixing learners' incorrect/broken 
[mental models](https://carpentries.github.io/instructor-training/02-practice-learning.html#building-a-mental-model) 
is as important as presenting your learners with new knowledge and correct information. 
When mental models are broken, learning can occur slower than you might expect[^1]. 
The longer a prior incorrect model is in use, and the more extensively it has to be "unlearned", 
the more it can actively interfere with the incorporation of the new correct knowledge 
(since it will contradict the misconceptions already present in the mental model).

### Example Misconceptions

#### Everyday Life Example

An example misconception from everyday life ([borrowed from The Carpentries Instructor Training](https://carpentries.github.io/instructor-training/instructor/02-practice-learning.html#misconceptions)) is, knowing that a 
bigger object (more volume) pushes out more water out of a basin than a smaller object (less volume), 
assuming that the similar principle will apply for objects of different weights. Surprisingly, 
heavier objects of the same volume as lighter ones will not push out more water.
![A misconception on how objects' mass affects the amount of water it can 'push out'](https://carpentries.github.io/instructor-training/fig/ballwater3a.svg){alt='Four sets of words inside rectangles, with labeled arrows connecting them. "Ball" is at the left, and "Water", at right. "Big Ball" and "Small Ball" are stacked vertically between them. Arrows from "Ball" are labeled with "Heavy Ball" and "Light Ball", and arrows to "Water" are labeled as "Pushes out MORE" and "Pushes out "LESS. There is a red "X" over the arrows labeled "Pushes out MORE" and "Pushes out LESS"'}

#### Coding Example

Another misconception, sometimes encountered by people who are learning programming languages
such as R and Python having used spreadsheets, is that variables in programs calculated by 
referencing other variables in formulas will retain the connection and be updated automatically 
when the referenced variables change. Variables in R or Python programs can use other variables 
in calculations (e.g. `a = b + 3`), but they do not behave like cells in spreadsheets
and updating the value of variable `b` after the previous assignment will not change the value of `a`.

#### Copyright / Licencing Example

Misconceptions often arise around topics of copyright and licencing of work/content (e.g. data, 
software, written material). Copyright allows a creator to state that they own the work they have created. This declaration is optional - even if the creator does not explicitly assert it, copyright of the work exists from the moment of creation. A licence is a legal document which sets down the terms under which the creator is releasing what they have created for others to use, modify, extend or exploit.
If this information is not provided, some will not reuse the work at all while others will assume they are free to do whatever they want with the work (as there is nothing to say that they cannot). This former is the correct assumption, even if this was not the intention of the copyright owner.


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: misconceptions (5 minutes)

What are the common misconceptions learners can have about the topic of your lesson?
How might you identify that misconception in your learners while they follow your lesson?
Share your answer in the collaborative notes document.

Hint: Try thinking about related or common tools the learners might know and how
applying that prior knowledge might lead to a misconception with
the topic you are teaching.

::::::::::::::::::::::::::::::::::::::::::::::::::
            
###  Multiple Choice Questions (MCQs)

[Multiple choice question (MCQ)](https://carpentries.github.io/instructor-training/02-practice-learning.html#using-formative-assessment-to-identify-misconceptions) exercises are types of a formative assessment that can help you target anticipated misconceptions. When designed carefully, each incorrect answer in a MCQ will have diagnostic power and provide valuable insight into how a mental model is broken. For example, suppose we are teaching children multi-digit addition. An example of a well-designed MCQ ([borrowed from The Carpentries Instructor Training](https://carpentries.github.io/instructor-training/02-practice-learning.html#using-formative-assessment-to-identify-misconceptions)) in this case could be:

_MCQ: What is 27 + 15?_

a) 42
b) 32
c) 312
d) 33

The correct answer is 42, but each of the other answers provides a valuable insight:

b) they do not understand the concept of a carry and are throwing it away completely
c) they understand the concept of a carry and know that they cannot just discard the carried ‘1’, but do not understand that it is actually a ten and needs to be added into the next column - they are treating each column of numbers as unconnected to its neighbours.
d) they understand that they need to carry ‘1’ but are adding it to the wrong column.

Their diagnostic power means that each of the wrong choices helps an instructor figure out precisely what misconceptions learners had adopted and in which ways their mental models are broken. As a result the instructor may decide to review a particular concept or change the pace of instruction. At the same time, learners get feedback about what they have misunderstood and what they need to focus their study efforts on - we call this **guided practice**.

### Choosing Plausible Distractors

When using a multiple choice question for formative assessment,
the incorrect answers you provide as options are _at least as important_ as the correct answer
because they offer the most useful insight into the mental model your audience is building.
But choosing incorrect answers can be difficult, especially early in a lesson where you are more likely
to encounter misconceptions that learners have arrived with
as opposed to those they have picked up while following the lesson.

:::::::::::::::::::::::::::::::: callout

## Prior Knowledge and Plausible Distractors

When identifying plausible distractors,
it is essential to consider the prior knowledge you expect learners to have of your lesson topic.

The plausible distractors in the MCQ example above
are chosen on the assumption that learners have been taught
addition by "carrying" numbers:
the incorrect answers are designed to diagnose misconceptions
associated with that method.

However, as [pointed out by Maneesha Sane](https://github.com/carpentries/instructor-training/issues/1403), 
if a learner has been taught to add numbers by another method,
e.g. first rounding them up or down to values that are more easy to remember and combine
(e.g. 27 to 30),
they might have misconceptions that cause them to arrive at an answer that is incorrect 
but not represented in the MCQ options.

::::::::::::::::::::::::::::::::::::::::
                    
### Example MCQs

#### Coding MCQ

Thinking back of the misconceptions of how values are assigned, referenced and updated in programming languages, 
here is an example MCQ that can probe learners for such misconceptions. 

_MCQ: Look at the following 3 assignment statements in Python._

```python
n = 300
m = n
n = -100
```

_What is the result at the end of the above assignments?_

a) n = 300 and m = 300
b) n = -100 and m = 300
c) n = -100 and m = -100
d) n = 200 and m = -100

The correct answer is b., while plausible distractors identify different misconceptions:

a\) they understand the value held by `n` is now also held by `m` but do not understand the value of `n` has 
been updated since the initial assignment (e.g. treating it as a constant).
c\) they do not understand `n` and `m` are separate variables/containers for values (which can hold the same values) 
but rather assume that `m` is referencing variable `n` instead of copying its value at the time of assignment 
(e.g. behaving as a reference to another cell in a spreadsheet).
d\) they think that the reassignment for `n` actually subtracts `100` from the original value.

#### Copyright / Licencing MCQ

An example MCQ to check on people's misconceptions around licencing and reusing other people's work
could be designed as follows.

_MCQ: Which of the following statements are true and which are false?_
   
a) I don’t need permission because I am only using the copyrighted work in educational or non-profit purposes  
b) I should always know the licence of any code, data, libraries, pictures or other work that you reuse or redistribute  
c) Since I’m planning to give credit to the authors who created the work I reuse, I do not have to worry about or need permission  
d) Material I obtain from the Internet is publicly accessible so no explicit permission is required  
e) The work I want to use does not have a copyright notice on it, so it’s not protected by copyright and I’m free to use it


The correct answers are as follows:

a) False - you always need an explicit permission from the creator to use their work.  
b) True - you should make sure that you have the permission for all the work that you are reusing, modifying or sharing.  
c) False - if you give credit to a work’s owner, that only means you are not plagiarising other 
people's work and claiming it as your own, however that does not mean that you have the permission to use it.  
d) False - publicly accessible work is not the same the work in the public domain. The owner 
explicitly must put their work in the public domain but attaching the appropriate licence to it, before you can freely reuse it. 
e) False - the use of copyright notice is optional as copyright exists implicitly from the moment the work is created.


To help identify plausible distractors, 
you can think about problems or questions from previous training events and what people struggled with, 
think about your own misconceptions in the past,
or ask colleagues about their experiences. 
It is important to consider [_expert awareness gap_][expert-awareness-gap-instructor-training],
the phenomenon where experts in a topic forget what it is like not to have a good mental model of it.
Observing how others learn your topic and asking colleagues to review lesson content as you design it
can help mitigate this.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: designing a diagnostic exercise (30 minutes)

Create a multiple choice question (MCQ) that could be used in your lesson,
to detect the misconception you identified above.
As well as the correct answer,
include 1-3 answer options that are not obviously incorrect (*plausible distractors*)
and have *diagnostic power*
i.e. each incorrect answer helps you pinpoint the exact misconception carried by the learner.
Write down what misconception is being tested for each incorrect answer.

If you are working on your lesson with others, swap with a partner and review each other's MCQs, considering the following questions:

- Is the question clear and easy to understand? Could the wording be improved in some way?
- Are the incorrect answers to the MCQ plausible distractors?
- Do the incorrect answers provide diagnostic power, to help an Instructor identify the misconception the learner has?
- Are there any incorrect answers missing i.e. are there other misconceptions that could be detected with this MCQ?

::::::::::::::::::::::::::::::::::::::::::::::::::

### Multiple Choice Questions for Assessing Higher Cognitive Skills
One common misconception about multiple choice questions is that they can be used only to test the ability to recall information or explain concepts, and are not suitable for assessing higher cognitive skills such as analysis or evaluation of information.

However, when supported by the appropriate scaffolding of information and context, multiple choice questions can be designed to exercise and assess these skills. Consider this advice, from [_Is This a Trick Question?_][trick-question] (page 19):

> One way to write multiple choice questions that require more than recall is to develop questions that resemble miniature "cases" or situations. Provide a small collection of data, such as a description of a situation, a series of graphs, quotes, a paragraph, or any cluster of the kinds of raw information that might be appropriate material for the activities of your discipline.
> 
> Then develop a series of questions based on that material. These questions might require students to apply learned concepts to the case, to combine data, to make a prediction on the outcome of a process, to analyze a relationship between pieces of the information, or to synthesize pieces of information into a new concept.

Just like the other exercise types explored in the main curriculum, designing effective multiple choice questions can be difficult but it is worth persevering with: a good set of exercises is a great asset to a lesson and especially helpful to instructors teaching it.

[^1]: See chapter 1, _How Does Students' Prior Knowledge Affect Their Learning?_,
      of [Ambrose et al. 2010](learners/reference.md#litref).
