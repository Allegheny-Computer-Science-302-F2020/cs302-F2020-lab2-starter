# cs302-F2020-lab2-starter

![](../../workflows/build/badge.svg)

## Table of Contents

* [Objectives](#objectives)
* [Introduction](#introduction)
* [Continuous Learning](#continuous-learning)
* [Assignment Reminders](#assignment-reminders)
* [Accessing the Assignment](#accessing-the-assignment)
* [Laboratory Assignment Tasks](#laboratory-assignment-tasks)
  + [Create a Travel Photographs Web Site](#create-a-travel-photographs-web-site)
  + [Running a Web Server](#running-a-web-server)
  + [Reflecting on the Laboratory Assignment](#reflecting-on-the-laboratory-assignment)
  + [Transferring Your Source code, Technical Writing, and Screenshot to GitHub](#transferring-your-source-code-technical-writing-and-screenshot-to-github)
* [Automated Checks with GatorGrader](#automated-checks-with-gatorgrader)
* [Assignment Assessment](#assignment-assessment)
* [Advance Feedback on an Assignment](#advance-feedback-on-an-assignment)
* [Discussion of a Graded Assignment](#discussion-of-a-graded-assignment)
* [Additional Resources](#additional-resources)
  + [System Commands](#system-commands)
  + [Using Docker](#using-docker)
  + [Using the Docker Shell](#using-the-docker-shell)
  + [Downloading Project Updates](#downloading-project-updates)
  + [Using GitHub Actions](#using-github-actions)
  + [System Requirements](#system-requirements)
  + [Reporting Problems](#reporting-problems)
  + [Receiving Assistance](#receiving-assistance)

## Objectives

The learning objectives for this laboratory assignment are as follows:

- To configure Git and GitHub on your laptop and on the GitHub servers
- To transfer files from your laptop to your GitHub repository
- To use your text editor to manipulate code blocks in a Markdown file
- To use a Docker container to run the automated checks performed by GatorGrader
- To use a terminal window to run a web server through a Python program and observe its output
- To use HTML source code to program a complete and correct web page
- To make references to resources in the HTML source code of a web page
- To use HTML linting tools to preemptively detect potential defects in a web page

## Introduction

Designed for use with [GitHub Classroom](https://classroom.github.com/) and
[GatorGrader](https://github.com/GatorEducator/gatorgrader/), this repository
contains a laboratory assignment for a web development course. The source code
and technical writing for this assignment must pass tests set by the
[GatorGrader tool](https://github.com/GatorEducator/gatorgrader). When you use
the `git commit` command to transfer your source code to your GitHub
repository, GitHub Actions will initialize a build of your assignment, checking
to see if it meets all of the requirements. If both your source code and
writing meet all of the established requirements, then you will see a green ✔
in the listing of commits in GitHub. If your submission does not meet the
requirements, a red ❌ will appear instead. Please note that, at the option of
the course instructor, some checks may be run in GitHub Actions that are not
run locally by the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader).

## Continuous Learning

If you have not done so already, please read all of the relevant [GitHub
Guides](https://guides.github.com/) that explain how to use many of the features
that GitHub provides. In particular, please make sure that you have read the
following GitHub guides: [Mastering
Markdown](https://guides.github.com/features/mastering-markdown/), [Hello
World](https://guides.github.com/activities/hello-world/), and [Documenting Your
Projects on GitHub](https://guides.github.com/features/wikis/). Each of these
guides will help you to understand how to use both [GitHub](http://github.com) and
[GitHub Classroom](https://classroom.github.com/).

Students who want to learn more about how to use
[Docker](https://www.docker.com) should review the [Docker
Documentation](https://docs.docker.com/). Students are also encouraged to
review the documentation for their text editor, which is available at [VS
Code](https://code.visualstudio.com/docs). You should also review the [Git
documentation](https://git-scm.com/doc) to learn more about how to use the Git
command-line client. In addition to talking with the instructor and technical
leader for your course, students are encouraged to search
[StackOverflow](https://stackoverflow.com/) for answers to their technical
questions.

As outlined in the course schedule in the [course planning
repository](https://github.com/Allegheny-Computer-Science-302-F2020/cs302-F2020-plans),
students should also read all of the assigned readings for up to and including
the week of the semester on which this laboratory assignment was assigned.

## Assignment Reminders

- **Follow each step carefully**. Slowly read each sentence in this document,
  making sure that you precisely follow each instruction. Take notes about each
  step that you attempt, recording your questions and ideas and the challenges
  that you faced. If you are stuck, then please tell a technical leader or the
  course instructor what assignment step you recently completed.

- **Regularly ask and answer questions**. Please log into Slack at the start of
  the laboratory session and then join the appropriate channel. If you have a
  question about one of the steps in an assignment, then you can post it to the
  designated channel, discussing your questions through both Slack and the
  Google Meet designated for the class.

- **Store your files in GitHub**. Starting with this laboratory assignment, you
  will be responsible for storing all of your files (e.g., Python source code
  and Markdown-based writing) in a Git repository using GitHub Classroom. Please
  verify that you have saved your source code in your Git repository by using
  `git status` to ensure that everything is updated. You can see if your
  assignment submission meets the established correctness requirements by using
  the provided checking tools on your local computer and by checking the commits
  in GitHub.

- **Keep all of your files**. Don't delete your programs, output files, and
  written reports after you submit them through GitHub; you will need them
  again when you study for the course assessments and work on the other
  laboratory, practical, and technical challenge assignments.

- **Hone your technical writing skills**. Computer science assignments require
  to you write technical documentation and descriptions of your experiences when
  completing each task. Take extra care to ensure that your writing is
  interesting and both grammatically and technically correct, remembering that
  computer scientists must effectively communicate and collaborate with their
  team members and the student technical leaders and course instructor.

- **Review the Honor Code on the syllabus**. While you may discuss your
  assignments with others, copying source code or technical writing is a
  violation of Allegheny College's Honor Code.

## Accessing the Assignment

To access this assignment, you should go into the `#announcements` channel in
our Slack workspace and find the announcement that provides a link for it. Copy
this link and paste it into your web browser. Now, you should accept the
laboratory assignment and see that GitHub Classroom created a new GitHub
repository for you to access the assignment's starting materials and to store
the completed version of your assignment. Specifically, to access your new
GitHub repository for this assignment, please click the green "Accept" button
and then click the link that is prefaced with the label "Your assignment has
been created here". If you accepted the assignment and correctly followed these
steps, you should have created a GitHub repository with a name like
`Allegheny-Computer-Science-302-Fall-2020/computer-science-302-fall-2020-lab-2-gkapfham`.
Unless you provide the course instructor with documentation of the extenuating
circumstances that you are facing, not accepting the assignment means that you
automatically receive a failing grade for all of its components.

Before you move to the next step of this laboratory assignment, please make sure
that you read all of the content on the web site for your new GitHub repository,
paying close attention to the technical details about the commands that you will
type and the output that your program must produce. Now you are ready to
download the starting materials to your laboratory computer. Click the "Clone or
download" button and, after ensuring that you have selected "Clone with SSH",
please copy this command to your clipboard. At this point, you can open a new
terminal window and type the command `mkdir cs302F2020`. To enter into this
directory you should now type `cd cs302F2020`. Next, you can type the either
`ls` (on either MacOS or Linux) or `dir` (on Windows 10 Pro or Windows 10
Enterprise) and see that there are no files or directories inside of this
directory. By typing `git clone` in your terminal and then pasting in the string
that you copied from the GitHub site you will "download" all of the code for
this assignment. For instance, if the course instructor ran the `git clone`
command in the terminal, it would look like:

```
git clone git@github.com:Allegheny-Computer-Science-302-F2020/computer-science-302-fall-2020-lab-2-gkapfham.git
```

After this command finishes, you can use `cd` to change into the new directory.
If you want to "go back" one directory from your current location, then you can
type the command `cd ..`. Finally, please continue to use the `cd` and `ls`
commands to explore the files that you automatically downloaded from GitHub. If
one of the aforementioned commands does not work correctly, then it is possible
that your terminal window is not up-to-date or not configured correctly. In this
case, please share your specific error messages with the instructor, ultimately
working to master the use of terminal commands. What files and directories do
you see? What do you think is their purpose? Spend some time exploring, telling
your discoveries to a student technical leader.

## Laboratory Assignment Tasks

### Create a Travel Photographs Web Site

This laboratory assignment invites you to implement a web site using the HTML
programming language. Specifically, you will create an extended version of the
travel photographs web site that looks like the one in the
[screenshot](images/travels_example.png) in the `images/` directory of your
repository. To start this step of the assignment, you will need to include the
cascading style sheet (CSS) that controls, for instance, the fonts on the web
site. You can achieve this step by adding the code `<link href="css/github.css"
rel="stylesheet">` to the `<head>` region of the `src/www/index.html` file.
Note that you also need to have another line of source code to load the
`emoji.css` file and its features for including an emoji in a web site. How
would you write that line of HTML source code? To get started you can refer to
example of how to include the two required CSS files in your
`src/www/index.html` file in the following code segment:

```
  <head>
    <meta charset="utf-8"/>
    <meta name="viewport" content="width=device-width"/>
    <link href="css/github.css" rel="stylesheet">
    <link href="css/emoji.css" rel="stylesheet">
    <title>Share Your Travels</title>
  </head>
```

At this point, you are ready to add, in the `<body>` region of the `index.html`
file, the code needed to display the provided image that is in the `img/`
directory. Can you find the source code location where this file name and
directory must be included? Using the textbook's content in Figure 3.16 and
Table 3.1, can you write the correct source code that includes the image? Now,
you are ready to add the five reviews of the photograph. You should include a
customized version of this source code in your own web site, changing the name,
time, and emoji to appropriate values. To learn more about each emoji that is
available for inclusion in your web site, please visit [Emoji
CSS](https://afeld.github.io/emoji-css/). Ultimately, your web site should
contain at least five photograph reviews that follow the format given in the
following code segment. Finally, students should check the correctness of their
HTML by running the command `htmlhint src/www/index.html` in their terminal
window, upon entering into the Docker container. Finally, if the web site
displays incorrectly in your web browser or the `htmlhint` tool reveals errors
then you should fix them until your web pages looks similar to the one in the
provided screenshot.

```
<blockquote>
  <p><b>By Ricardo on <time>February 8, 2018</time></b></p>
  <p>Wow, that is a great photograph. How did you take it?</p>
  <p>I would describe this photograph as <i class="em em---1"></i> </p>
</blockquote>
```

### Running a Web Server

Your GitHub repository contains an file called `index.html` in the `src/www`,
which is the root of your web server. Here is the command to type in your
terminal window for starting the HTTP server using the Python programming
language on your laptop:

```
python -m http.server --directory src/html/learning-objectives
```

Please note that it is possible that your web server will display errors about
its inability to find certain files. However, as long as those files are not the
HTML or CSS files that are the focus of this assignment, your project should
display correctly. With that said, if your web server reports that it cannot
find files like `index.html` or `css/github.css` then you need to confirm that
your server is running in the correct directory.

### Reflecting on the Laboratory Assignment

Once you have finished both of the previous technical tasks, use your text
editor to answer all of the questions in the `writing/reflection.md` file. For
instance, you should explain the meaning of the three provided commands and
answer all of the other questions about your experiences in completing this
laboratory assignment.

### Transferring Your Source code, Technical Writing, and Screenshot to GitHub

As you are working on your laboratory assignment, please make sure that you use
VSCode to regularly save your work and transfer it to the GitHub servers. For
instance, please use the `git commit` command in your terminal window or use the
similar feature in VSCode to "stage" your changes in your repository. Once you
have committed your source code to your repository, you can use the `git push`
command to transfer your work to your GitHub repository, making it available for
the course instructor to assess. Please make sure that you regularly commit your
source code and technical writing, using descriptive commit messages to explain
how each commit changes the contents of the repository.

After you have finished your web page, please make sure that you take a
screenshot of it, either using a tool built into your browser or your operating
system. You should save your screenshot in the `images/travels_submission.png`
file taking care to store the file in the correct directory and to give it the
requested file name extension. As you are completing the work for this
assignment, make sure that your build in GitHub Actions is passing and that your
HTML source code passes all of the linting checks performed by `htmlhint` and
the additional checks run by GatorGrader, as described in the next section.

## Automated Checks with GatorGrader

In addition to meeting all of the requirements outlined in this assignment
sheet, your submission must pass the following checks that
[GatorGrader](https://github.com/GatorEducator/gatorgrader) automatically
assesses:

If [GatorGrader's](https://github.com/GatorEducator/gatorgrader) automated
checks pass correctly, the tool will produce the output like the following in
addition to returning a zero exit code (which you can access by typing the
command `echo $?`). You will need to run
[GatorGrader](https://github.com/GatorEducator/gatorgrader) in a Docker
container by following the steps in the [Using Docker](#using-docker) section.

- The command `htmlhint src/www/index.html` executes correctly
- The command output has exactly 1 lines
- The file emoji.css exists in the src/www/css directory
- The file github.css exists in the src/www/css directory
- The file index.html exists in the src/www/ directory
- The file plane.jpg exists in the src/www/img directory
- The file reflection.md exists in the writing directory
- The file travels_example.png exists in the images directory
- The file travels_submission.png exists in the images directory
- The index.html in src/www/ has at least 15 of the `<p>` fragment
- The index.html in src/www/ has at least 1 of the `<body>` fragment
- The index.html in src/www/ has at least 1 of the `emoji.css` fragment
- The index.html in src/www/ has at least 1 of the `github.css` fragment
- The index.html in src/www/ has at least 1 of the `<head>` fragment
- The index.html in src/www/ has at least 1 of the `<html>` fragment
- The index.html in src/www/ has at least 1 of the `utf-8` fragment
- The index.html in src/www/ has at least 5 of the `<blockquote>` fragment
- The index.html in src/www/ has at least 5 of the `i class` fragment
- The index.html in src/www/ has at least 5 of the `<time>` fragment
- The index.html in src/www/ has exactly 0 of the `Add Your Name Here` fragment
- The index.html in src/www/ has exactly 0 of the `TODO` fragment
- The index.html in src/www/ has exactly 1 of the `<h1>Share Your Travels</h1>` fragment
- The index.html in src/www/ has exactly 1 of the `<h3>Reviews</h3>` fragment
- The index.html in src/www/ has exactly 1 of the `<title>Share Your Travels</title>` fragment
- The reflection.md in writing has at least 600 word(s) in total
- The reflection.md in writing has at least 6 of the `code` tag
- The reflection.md in writing has exactly 0 of the `Add Your Name Here` fragment
- The reflection.md in writing has exactly 0 of the `TODO` fragment
- The reflection.md in writing has exactly 10 of the `heading` tag
- The reflection.md in writing has exactly 1 of the `list` tag
- The reflection.md in writing has exactly 2 of the `code_block` tag
- The repository has at least 10 commit(s)

```
        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
        ┃ Passed 32/32 (100%) of checks for cs302-F2020-lab2! ┃
        ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
```

## Assignment Assessment

Taking inspiration from the principles of [specification-based
grading](https://www.amazon.com/Specifications-Grading-Restoring-Motivating-Students/dp/1620362422),
the grade that a student receives on a laboratory assignment will be based on
whether or not it meets the standards for technical work in the fields of
software engineering and discrete structures. Instead of receiving a single
numerical or letter grade for this assignment, your grade will have the
following components:

- **Percentage of Correct GatorGrader Checks Ranging Between 0 and 100**: Your
  submitted Python program must pass all of GatorGrader's checks by, for
  instance, ensuring that it produces the correct output and has all of the
  required characteristics. Your technical writing must pass all of
  GatorGrader's checks about, for instance, the length of its output and its use
  of the required Markdown language features for technical writing. For this
  component of a laboratory assignment's grade, your work will receive a
  percentage, ranging from 0 to 100, that corresponds to the percentage of
  GatorGrader checks that automatically pass inside of a GitHub Actions build.

- **GitHub Actions Build Status of Either ✔  or ❌**: Since additional checks on
  the Python source code and/or technical writing are encoded in GitHub Action
  workflows and, moreover, all of the GatorGrader checks are also run in GitHub
  Actions, your work will receive a checkmark grade if the last
  before-the-deadline build in GitHub Actions passes and a ✔  appears in the
  GitHub commit log instead of an ❌. The build status reported by GitHub
  Actions will only be a ✔ if the source code and technical writing in the
  GitHub repository pass all of both the GatorGrader checks and the additional
  checks.

- **Technical Writing Mastery of Either ✔  or ❌**: Students will also receive a
  ✔ grade when the responses to the technical writing questions presented in the
  `writing/reflection.md` reveal a mastery of technical writing skills. To
  receive a checkmark grade, the submitted writing should have correct spelling,
  grammar, punctuation, and formatting in addition to following the rules of the
  Markdown language. Your work will receive a ✔ grade for this component
  if the build report from GitHub Actions reveals that there are no detected
  mistakes in the technical writing.

- **Technical Knowledge and Skill Mastery of Either ✔  or ❌**: Students will
  also receive a checkmark grade when the GitHub repository reveals that they
  have mastered all of the technical knowledge and skills developed during the
  completion of the laboratory assignment. As a part of this grade, the
  instructor will assess aspects of the project including, but not limited to,
  the use of effective Python source code comments, correct Git commit messages,
  and accurate responses to the technical writing questions.

## Advance Feedback on an Assignment

Students who wish to receive feedback on their work for any course assignment
should first open an issue on the issue tracker for their assignment's GitHub
repository, giving an appropriate title and description for the type of feedback
that you would like the course instructor to provide. After creating this issue,
you will see that GitHub has created a unique web site that references it. To
alert the course instructor to the fact that the issue was created and that you
want feedback on your work, please send it to him by a Slack direct message at
least 24 hours in advance of the project's due date. After the instructor
responds to the issue, please resolve all of the stated concerns and participate
in the discussion until the issue is resolved and ultimately marked as closed.

## Discussion of a Graded Assignment

Students who wish to receive feedback on their work for any graded course
assignment should leave question in the same region of Github where the course
instructor submitted the assignment's grade. For example, if the instructor
submits your grade to a pull request in your repository for a laboratory
assignment, then you should ask questions about your grade in that pull request,
bearing in mind the need to @-mention the course instructor in the body of your
comment. Students can continue to discuss the graded assignment with the course
instructor until they understand all the technical topics that were the
focus of the particular assignment.

## Additional Resources

### System Commands

This project invites students to enter system commands into a terminal window.
This assignment uses [Docker](https://www.docker.com) to deliver programs, such
as `gradle` and the source code and packages needed to run
[GatorGrader](https://github.com/GatorEducator/gatorgrader), to a students'
computer, thereby eliminating the need for a programmer to install them on their
development workstation. Individuals who do not want to install Docker can
optionally install of the programs mentioned in the [Project
Requirements](#requirements) section of this document.

### Using Docker

Once you have installed [Docker
Desktop](https://www.docker.com/products/docker-desktop), with MacOS and Linux
you can use the following `docker run` command to start `gradle grade` as a
containerized application, using the
[DockaGator](https://github.com/GatorEducator/dockagator) Docker image available
on
[DockerHub](https://cloud.docker.com/u/gatoreducator/repository/docker/gatoreducator/dockagator).

```bash
docker run --rm --name dockagator \
  -v "$(pwd)":/project \
  -v "$HOME/.dockagator":/root/.local/share \
  gatoreducator/dockagator
```

The aforementioned command will use `"$(pwd)"` (i.e., the current working
directory) as the project directory and `"$HOME/.dockagator"` as the cached
GatorGrader directory. Please note that both of these directories must exist,
although only the project directory must contain something. Generally, the
project directory should contain the source code and technical writing for this
assignment, as provided to a student by the instructor through GitHub.
Additionally, the cache directory should not contain anything other than
directories and programs created by DockaGator, thus ensuring that they are not
otherwise overwritten during the completion of the assignment. To ensure that
the previous command will work correctly, you should create the cache directory
by running the command `mkdir $HOME/.dockagator` on the MacOS and Linux
operating systems. However, if you are using the Windows operating system then
you will instead need to type the command `mkdir
%HomeDrive%%HomePath%/.dockagator`. Finally, if the above `docker run` command
does not work correctly on the Windows operating system, you may need to instead
run the following command to adapt to the differences in the `cmd` terminal
window:

```bash
docker run --rm --name dockagator \
  -v "%cd%:/project" \
  -v "%HomeDrive%%HomePath%/.dockagator:/root/.local/share" \
  gatoreducator/dockagator
```

Here are some additional commands that you may need to run when using Docker:

* `docker info`: display information about how Docker runs on your workstation
* `docker images`: show the Docker images installed on your workstation
* `docker container list`: list the active images running on your workstation
* `docker system prune`: remove many types of "dangling" components from your workstation
* `docker image prune`: remove all "dangling" docker images from your workstation
* `docker container prune`: remove all stopped docker containers from your workstation
* `docker rmi $(docker images -q) --force`: remove all docker images from your workstation

### Using the Docker Shell

Since the above `docker run` command uses a Docker images that, by default, runs
`gradle grade` and then exits the Docker container, you may want to instead run
the following command so that you enter an "interactive terminal" that will
allow you to repeatedly run commands within the Docker container. Don't forget
that, if you are using the Windows operating system, then you will need to use a
different command to run Docker, as explained previously in this document.

```bash
docker run -it --rm --name dockagator \
  -v "$(pwd)":/project \
  -v "$HOME/.dockagator":/root/.local/share \
  gatoreducator/dockagator /bin/bash
```

Once you have typed this command, you can use the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader) in the Docker container by
typing the command `gradle grade` in your terminal. Running this command will
produce a lot of output that you should carefully inspect. If GatorGrader's
output shows that there are no mistakes in the assignment, then your source code
and writing are passing all of the automated baseline checks. However, if the
output indicates that there are mistakes, then you will need to understand what
they are and then try to fix them.

To run one of these commands, you must be in the main (i.e., "home base")
directory for this assignment where the `build.gradle` file is located. Finally,
please note that students who are using Windows 10 Pro may need to run the
Windows versions of these commands on a long single line in the terminal window.

### Downloading Project Updates

If the course instructor pushes updates to this assignment and you received it
through GitHub Classroom and you would like to also receive these updates, then
you can type this command in the main directory for this assignment:

```
git remote add download git@github.com:Allegheny-Computer-Science-302-F2020/cs302-F2020-lab2-starter/
```

You should only need to type this command once; running the command additional
times may yield an error message but will not negatively influence the state of
your Git repository. Now, you are ready to download the updates provided by the
GatorGrader maintainers by typing this command:

```
git pull download master
```

This second command can be run whenever the course instructor needs to provide
you with new source code for this assignment. However, please note that, if you
have edited the files that we updated, running the previous command may lead to
Git merge conflicts. If this happens, you may need to manually resolve them with
the help of the instructor or a student technical leader. Finally, please note
that the [Gradle plugin](https://github.com/GatorEducator/gatorgradle) for
[GatorGrader](https://github.com/GatorEducator/gatorgrader) will automatically
download the newest version of GatorGrader.

### Using GitHub Actions

This assignment uses [GitHub Actions](https://github.com/features/actions) to
automatically run [GatorGrader](https://github.com/GatorEducator/gatorgrader)
and additional checking programs every time you commit to your GitHub
repository. The checking will start as soon as you have accepted the assignment
&mdash; thus creating your own private repository &mdash; and the course
instructor and/or GitHub enables GitHub Actions on it. If you do not see either
a yellow &#9679; or a green ✔ or a red ❌ in your listing of commits, then
please ask the course instructor to see whether or not GitHub Actions was
correctly enabled.

### System Requirements

This assignment was developed to work with the following software and versions:

- Docker Desktop
- Operating Systems
  - Linux
  - MacOS
  - Windows 10 Pro
  - Windows 10 Enterprise
- Programming Language Tools
  - Gradle 6.6
  - MDL 0.5.0
  - Python 3.7 or 3.8

### Reporting Problems

If you have found a problem with this assignment's provided source code or
documentation, then you can go to the [Computer Science 302 Fall 2020 Planning
Repository](https://github.com/Allegheny-Computer-Science-302-F2020/cs302-F2020-plans)
and [raise an
issue](https://github.com/Allegheny-Computer-Science-302-F2020/cs302-F2020-plans/issues).
If you have found a problem with the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader) and the way that it checks
your assignment, then you can also [raise an
issue](https://github.com/GatorEducator/gatorgrader/issues) in that repository.
To ensure that your issue is properly resolved, please provide as many details
as is possible about the problem that you experienced. Individuals who find, and
use the appropriate GitHub issue tracker to correctly document, a mistake in any
aspect of this assignment will receive extra credit towards their grade for the
course.

### Receiving Assistance

If you are having trouble completing any part of this project, then please talk
with either the course instructor or a student technical leader during the
course session. Alternatively, you may ask questions in the Slack workspace for
this course. Finally, you can schedule a meeting during the course instructor's
office hours.
