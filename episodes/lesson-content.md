---
title: Adding Lesson Content
teaching: 15
exercises: 40
start: yes
---

::::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Add lesson episodes as individual pages of a lesson website.
- Use _fenced divs_ to create different structural elements within a page to 
format objectives, questions, keypoints, exercises and their solutions in a lesson website.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How do you create and modify the pages in a lesson?
- How should different structural elements be presented in a lesson website?

::::::::::::::::::::::::::::::::::::::::::::::::::


Now that we have completed the basic configuration of a lesson site,
it is time to move on and look at where the actual lesson content will be written.

## Lesson Home Page

The "home page" of a lesson is created from the `index.md` file:
this file should contain a brief introduction to the lesson,
designed to give visitors to the page a first impression of the lesson
and whether it is appropriate for them.
The file begins with a short header,
written in the same key-value pair syntax we encountered in `config.yaml`.

```markdown
---
site: sandpaper::sandpaper_site
---

```

This header configures how the site will be built by `sandpaper`,
one of the components of The Carpentries Workbench,
and should be left untouched.
The page content begins after the blank line that follows this header.

:::::::::::::::::::::::::::::::: spoiler

### Markdown Rendering on GitHub

You might have noticed by now that GitHub provides
a preview of content in Markdown files,
and displays an interpreted ("rendered") version of Markdown file content
by default in its web interface.
You might also notice that the content of `index.md` is displayed differently
when viewed on GitHub
from how it appears on the homepage of your lesson website:
the header mentioned above appears in a tabular layout on GitHub,
but is not visible on the lesson homepage.

This is because the lesson infrastructure accepts an expanded set of
elements in the source Markdown files:
syntax for components of a lesson website
that are not part of the standard set of Markdown features,
e.g. page metadata such as the YAML header above,
or blocks to make exercises and solutions visually distinctive.
In these cases, you may see GitHub render the content differently
from how it appears on your website, or not at all.

We will encounter more examples of this throughout the lesson,
but the important thing to remember for now is that
**how GitHub displays source (R) Markdown files is not a reliable indicator
of how content will be displayed in your website**.

::::::::::::::::::::::::::::::::::::::::

To get started on this home page,
replace the template text with
the same short description you added to your `README.md`.

Below those, you can add the prerequisite skills you determined earlier for your lesson,
as a bullet point list to `index.md`:

```markdown
- prerequisite 1
- prerequisite 2
- ...
```

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: practice editing Markdown in GitHub (optional)

Add the objectives you defined for your lesson
as a bullet list in the `index.md` file of your lesson repository.


::::::::::::::::::::::::::::::::::::::::::::::::::

## Episodes

As we've discussed previously, the main body of the lesson is written in _episodes_:
the individual chunks or sections that the lesson is separated into.
The episode pages of the lesson site will be constructed from Markdown or RMarkdown files
in the `episodes` folder of the lesson repository.

The `episodes` folder of the new repository contains a single file,
`introduction.md`.
The content of this file includes examples of how to write Markdown files
for The Carpentries Workbench.

There are two important things to note:

1. Like `index.md`, the episode file begins with a short header.
   The fields in this header describe the episode title and the estimated time (in minutes)
   required to teach it and complete the exercises.
2. The example content includes several lines that start with strings of colons (`:::::::`).
   These mark the beginnings and ends of structural elements within the page,
   called _fenced divs_, which get rendered in a visually distinct way on the lesson website.
   Each fenced div starts and ends with a string of at least 3 colons (":::") and 
   the word at the end of the starting colons (the fenced div's tag) indicates what kind of block it is.
   [There are many types of fenced divs in the lesson infrastructure](https://carpentries.github.io/sandpaper-docs/instructor/component-guide.html#callout-blocks) 
   and we will explore some of them in this episode.

### Creating a new episode

Let's create a new episode file, for one of the episodes you have just identified.
First, open the "raw" view of the `introduction.md` example episode,
and copy its contents.

```markdown
---
title: "Intro to Markdown"
teaching: 10
exercises: 2
---

:::::::::::::::::::::::::::::::::::::: questions 

- How do you write a lesson using Markdown and `{sandpaper}`?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Explain how to use markdown with The Carpentries Workbench
- Demonstrate how to include pieces of code, figures, and nested challenge blocks

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

This is a lesson created via The Carpentries Workbench. It is written in
[Pandoc-flavored Markdown](https://pandoc.org/MANUAL.txt) for static files and
[R Markdown][r-markdown] for dynamic files that can render code into output. 
Please refer to the [Introduction to The Carpentries 
Workbench](https://carpentries.github.io/sandpaper-docs/) for full documentation.

...

::::::::::::::::::::::::::::::::::::: keypoints 

- Use `.md` files for episodes when you want static content
- Use `.Rmd` files for episodes when you need to generate output
- Run `sandpaper::check_lesson()` to identify any issues with your lesson
- Run `sandpaper::build_lesson()` to preview your lesson locally

::::::::::::::::::::::::::::::::::::::::::::::::
```

::: instructor

Be careful here to ensure that participants who are collaborating on the same repository
do not create conflicts e.g. by editing the same file or creating files with identical names.

:::


Now create a new file in the `episodes` folder.
Based on the episodes you planned out earlier,
choose a name for your episode that concisely describes the intended content,
e.g. `data-visualisation.md`
(or `data-visualisation.Rmd` for a lesson based on R Markdown).
It is vital to include the file extension when naming this file:
only files with the `.md` or `.Rmd` extensions will be built into
webpages by the lesson infrastructure.

For page content, paste the content the `introduction.md` file you copied earlier and:

1. replace the title in the header with the title of your episode
2. set the `teaching` and `exercises` fields to zero for now
3. replace the contents of the `questions` div with the questions for your episode you defined earlier
4. replace the contents of the `objectives` div with the episode-level objectives you defined earlier 
5. replace the contents of the `keypoints` div with the key points for your episode you defined earlier
6. Ignore or delete the rest of the content of the episode (i.e. only focus on the three structural elements - questions, objectives and keypoints).


```markdown
---
title: "Episode Title"
teaching: 0
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- question 1
- question 2
- ... 

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- objective 1
- objective 2
- ...

::::::::::::::::::::::::::::::::::::::::::::::::

Some episode content ...

::::::::::::::::::::::::::::::::::::: keypoints

- keypoint 1
- keypoint 2
- ...

::::::::::::::::::::::::::::::::::::::::::::::::

```

::: spoiler

### Full List of Fenced Divs

[The Workbench Component Guide][component-guide] provides a full list of
all the different classes of fenced div that can be included using the lesson infrastructure.
The guide specifies which divs are required for an episode
(`objectives`, `questions`, and `keypoints`),
and which are optional.

:::


### Adding a new episode to the lesson navigation

This new episode will not yet appear in the navigation of your lesson site.
To enable this, we need to specify where the episode should appear
in the order of the lesson.
That episode order is defined in the `episodes` field of the `config.yaml` file:

```YAML
# Order of episodes in your lesson
episodes:
- introduction.md

```

Add the name of the new episode file you created to this list in `config.yaml`
and commit this change, for example:

```yaml
# Order of episodes in your lesson
episodes:
- introduction.md
- data-visualisation.md

```

After the lesson site has been rebuilt on GitHub,
you should see the episode title appear under _Chapters_
in the left sidebar navigation of your lesson site
after refreshing the webpage.
Clicking on that title will take you to the episode page built from the file you created.
At the top of the page body, you will find the episode title
and an _Overview_ box containing a list of the questions and objectives
defined for the episode.
Later, we will add more content to your chosen episodes.

TODO add a labelled screenshot of a new episode page

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: practice creating episodes (10 minutes)

Repeat the steps you just saw, to create another new episode file
and add it to the lesson site navigation.
If you know what another episode in your lesson will be about,
create the page for that.
Otherwise, feel free to use any values you like for the file name and episode title.

::::::::::::::::::::::::::::::::::::::::::::::::::

Using this approach, we can build up our lesson one episode at a time.


## Adding Exercises

To create an exercise in The Carpentries Workbench,
we use another two types of 'fenced divs':

* `discussions`, where the main task is for participants to discuss a topic or prompt, and 
* `challenges`, where the main task is a problem to be solved.

For example, to start a challenge fenced div, use at least 3 colons, 
followed by the `challenge` tag.
Then the content of the challenge is included on the following lines.
Finally, you need to close the fenced div using another line with least 3 colons.

```markdown
:::::::::::::::::::::::::::::::::::::: challenge

### Challenge Title

Challenge text, code, and other information goes here

::::::::::::::::::::::::::::::::::::::::::::::::::

```

If you also want to include an expandable solution box for the challenge you can
nest a `solution` fenced div within the `challenge` div.
The format is the same as for a challenge except the fenced div tag is `solution` instead.
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


## Optional and Important Material

The Carpentries Workbench includes fenced divs for highlighting key material that should not be 
skipped during instruction, as well as optional content that can be covered if time permits.

::::::::::::::::::::::::::::::::::::::::  spoiler

## Using Spoilers for Optional Materials

Often lessons have more content than can be reasonably taught in the amount of time allotted.
This is especially true for collaboratively developed lessons as each contributor/instructor
may have additional items they'd like to see included, leading to "scope creep".

To address this issue, in many Carpentries lessons, spoiler boxes are used for asides and short tangents,
e.g. points that might be relevant to some audiences but are not essential to the flow of the lesson.
These spoilers should still be kept to a minimum as they can be disruptive to instructors and readers.

Note, this use of the spoiler box is to use the expandable box functionality as nothing will be "spoiled"
by expanding this box.
Also, note that the spoiler box titles should be very clear so instructors need not expand the spoiler to know if they want to teach that extra.


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::: callout

## Calling Attention to Important Points

For important points in the lesson, you can add them to a callout box to emphasize their
importance.

::::: spoiler

### Inconsistent use of spoiler vs callout

You may notice that many of the older lessons use callouts for both additional material
and to highlight important points interchangeably.  Spoilers were developed in 2023
to help with separating these two different use cases.

:::::::::::::

::::::::::::::::::

## Glossary of Terms 

You have already started on compiling a glossary of terms for your lesson. 
The Workbench offers a standardized location for lesson terminology: `learners/reference.md`.

::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: More Practice (15 minutes)

Use this time to add more content to your lesson site.
Generally speaking, you should try to transfer the drafted content from your lesson design notes into the lesson website.
Here are some suggestions for things you might try:

1. Add your list of prerequisite knowledge/skills as a fenced div with the `prereq` class to your `index.md` file.
2. [Add some tabbed content](https://carpentries.github.io/sandpaper-docs/episodes.html#tabbed-content) in your episode. 
3. Start a glossary of terms in the `learners/reference.md` file, referring to [the Workbench documentation on how to add a list of term definitions](https://carpentries.github.io/sandpaper-docs/editing.html#learners).
4. Look through the [Workbench component guide](https://carpentries.github.io/sandpaper-docs/instructor/component-guide.html) and try implementing some of the other flavours of fenced div.
5. Add a new Markdown file to the `learners/` or `instructors/` folder and see if you can find the built page in your lesson site.

::::::::::::::::::::::::::::::::::::::::::::::::::

## Troubleshooting the Lesson Build

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

### Troubleshooting the Lesson Build (~10 mins)

This is a good opportunity to pause and check in on
how well trainees' lesson builds are running.
If anyone is having trouble with their workflows,
ask them to share their screen
and try following the troubleshooting steps to diagnose and fix the issue.

This is also a good opportunity to show what the GitHub actions look like when they are in progress, 
succeed, or fail if you haven't already.

If all is well, and you are pressed for time, this section can be skipped.

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

Sometimes, formatting errors and typos in the files of your repository can
cause the process that builds your lesson website to fail.

You will likely first notice the failure to build the lesson if the lesson website is not showing the changes you made.
You may also receive an email from GitHub about the build failure if that is your preferred way of receiving notifications
(but it may take you some time to realise this).
The good thing is that GitHub keeps your previous lesson version online
until the error is fixed and a new build is completed successfully.
If you are not yet familiar with the GitHub interface,
it can be difficult to pinpoint the problem.

Here are some points of advice that you can follow to help
find and fix the problem when you notice the build process fail.

- When you first notice that there is a problem, **stop** editing your lesson:
  any subsequent changes that you make will not be included in your lesson site until
  the problem is fixed, and might introduce additional issues,
  making it more difficult to find the original cause.
- **Look at the history** of commits
  (the link with a reversing stopwatch icon and "NN commits"
  at the top of the listing of files and folders in the repository homepage).
  Is there a place where the build has a red cross instead of green circle?
  If so, click on that commit to look at the "diff"
  (where it shows which lines have been modified).
  The error is likely to have been introduced by these changes.
- **Ask for help**: you can open an issue on your repository and tag a member of
  The Carpentries team to ask for help finding the problem.
  Alternatively, you can also ask for help in The Carpentries
  Slack workspace.
  (More about communication channels for discussing lesson development coming later in this training.)
- Waiting for the GitHub Actions process that builds the website to run can be tedious,
  and slow down the process of troubleshooting:
  it can take a few minutes for the process to reach the point where it encounters the problem.
  It can be helpful to download the files for your lesson
  and try to **build a version of the website on your local computer**,
  where the build process will be much faster.
  The Workbench documentation provides
  [instructions for installing the infrastructure](https://carpentries.github.io/sandpaper-docs/#installation)
  and [building a local preview of the lesson website](https://carpentries.github.io/sandpaper-docs/introduction.html#preview).


[sandpaper-docs-learners]: https://carpentries.github.io/sandpaper-docs/editing.html#learners

:::::::::::::::::::::::::::::::::::::::: keypoints

- The main pages of a lesson website (lesson episodes) are created from individual Markdown or RMarkdown files in the `episodes` folder of a lesson repository
- Objectives, questions, keypoints, exercises (and solutions), and other "special" structural 
page elements (other than plain text) can be formatted using _fenced div_ blocks - they are rendered 
visually differently in the lesson website. 
- There are many types of [fenced divs](https://carpentries.github.io/sandpaper-docs/instructor/component-guide.html#callout-blocks) available to lesson developers.

::::::::::::::::::::::::::::::::::::::::::::::::::


[^1]: [Kirschner et al. 2006](learners/reference.md#litref)
