# Project Phases
The phases of our projects are described in
[another document](https://docs.google.com/document/d/1MGC8xPRhHqr7SbqFHh2k0Bmqo_4eyT2M3WzD8AjCBVg/edit),
here we will talk about how to follow up on the different phases.

## Kick Off

Check that everyone has done the tasks assigned in the kick-off, and that any
produced documents are made available to everyone.

## Discovery

Ensure that all the elements of discovery are discussed between the relevant
people as described in the
[workflow document](https://docs.google.com/document/d/1MGC8xPRhHqr7SbqFHh2k0Bmqo_4eyT2M3WzD8AjCBVg/edit#heading=h.quyk3gemme8s).
This is a key point where we
should be critical and see if we have gone beyond what was asked of us. We want
to build valuable projects and this depends on us challenging the premises and
coming up with creative and innovative solutions to solve the user needs.

In regards to the data discovery have we allowed time to identify things that
might be interesting and that the client wasn’t aware off? Is the data good
enough to do what we want to do? Are there any other datasets that we have
worked with in other projects that we could potentially use in the current one?
Are there points of contact with other ongoing projects?

## Data

Besides the interesting scientific questions related with data there are two
key questions that we need to ask straight away during discovery and data
handling phase: Is all the data available?; Is the data in a state that we can
work with?. If the answer to any of these questions is no, we will need to
bring it up with the client and discuss the timeline with them; these need to
be made available and be in a good state to start designing.

To keep track of data in each project it is recommended that we have an
inventory spreadsheet where the different datasets are listed and any relevant
metadata is captured (e.g.: state of the dataset; where can it be found; what
type of data it is; source; etc.). This document needs to be kept up to date
during the life of the project, so that we can always refer to it as necessary.

When there is the need to process the client’s data to use in the project any
scripts and instructions on how to run them and how to use the generated data
should be documented on a repository on Github. Typically this has been done
through the use of Jupyter notebooks, and our data scientists are quite
familiar with this. These notebooks can then be shared with the development
team to explain how to use the data, and regular communication between the
data team and the developers will ensure that all is clear and the project can
move forward.

As with the other areas of a project, a timeline should be defined for the
data processing part. This should be aligned with both the design and
development phases, so that both phases can be informed as needed.

## Design

At each review point of the design process there are a few things that are
important to check with different members of the team (research, development,
data):

- Do the designs meet the requirements for each page?
- Are the designs too complex for implementation? Are there simpler alternatives?
- Will the designs have a strong impact in performance of the application? Will we need to request a lot of data on specific pages?
- Are all the interactions thought through (e.g.: how will a set of filters work; what happens when you click a dropdown; etc.)
- Are we accounting for the different states of the application (e.g.: errors in a form; no data; too much data; very few data; etc.)?
- Are we innovating? Are we going beyond the standard approaches? Are we keeping a balance?

Some of the points above don’t have straight answers and might require
allowing more time for the design process, but it is important that they are
discussed so that the conditions are met for us to deliver a good
product.

## Development

### Development Kick-off

Ahead of development we should run a development kick-off meeting where we
review all the pages that will be implemented and discuss how to split them
into releases. Release planning needs to take into consideration the client’s
priorities, and the releases might need to be reviewed as the project goes on,
to make sure that we keep aligned with those priorities. During the release
planning there might be new questions appearing about the designs, these
should not be ignored as the designs are not really set in stone, and if there
are doubts or ways to improve them we should do it.

### Sprints

Having decided on the release schedule, the next organizing unit is the
sprint. Knowing what needs to be delivered next should allow the development
team to organize the work in one or two weeks sprints. This allows us to
deliver updates to the client and to keep them in the loop about what we are
doing, and also enable the review of priorities with each new delivery.

### Daily Meeting

It’s recommended that the project team holds a daily meeting where they can
report on what they’ve worked on and will be working on that day. This meeting
can be very valuable as it makes it possible to identify blockers, and
opportunities to share experience and to organize pairing sessions when
relevant. Having designers and data scientists on this meeting is also
recommended as this way interactions can be scheduled replacing ad-hoc
interruptions. The daily meeting is also a good place to update estimates of
ongoing tasks, which will help plan the next
sprints.

# Timeline

Each project should be tracked on the project’s timeline document with
information about its deliverables and key milestones. When a task is
delegated to a member of the team, they also inherit the responsibility to
keep the timeline up to date for their task. The timeline must be kept up to
date by either the project manager or project leads.

It is advised that this document be shared with the whole team so that
everyone knows what to expect on each project. Besides including it on the
intranet page this document can be shared on the team channel on Slack and
pinned so that it’s easy to find.

# Tools

## Basecamp

We use it to communicate with our clients' teams. Basecamp is where most of
our conceptual discussions take place and where high level tasks are maintained.

### Tips and Best practices

- When using basecamp you can tweak the list of who will receive email
notifications for your messages.It's a good practice to pick the correct list
of recipients, rather than sending a message to everyone on the project, so
that people aren't flooded by all messages.
- When ToDo lists are being used in a Basecamp project it's important to use
the assignment functionality. This should be set to the person you're
expecting an answer from and a rough deadline for when you’re expecting an
answer, so that conversations don't get lost without response.
- It is your responsibility to keep an eye on tasks assigned to you and to
answer to discussions when you are mentioned on them. So make sure to tweak
Basecamp's settings so that they suit your way of working. If you like emails,
get emails, if you don't, visit the website.
- If you are assigned to new tasks or brought in to some discussion but you are
busy with other more urgent tasks, it is a good practice to acknowledge the
assignment or message anyway, so that no one is left hanging. [e.g.: Thanks
for your message, I'm currently in the middle of something, but will look back
at this as soon as I can].
- If you feel that a task or message is better suited to be dealt with by
someone else make sure to assign them or let them know, as they might not have
been notified.

## Pivotal Tracker

Our default tool to manage internal tasks for each of our projects. The UI and
functionality might be overwhelming, but if we all use it the same way then we
should minimise confusion and increase usefulness.

One key thing to keep in mind is that this is an internal tool, we are the
ones driving it and so it's our responsibility to ensure that it is useful for
us. However many of our boards are ‘public’ so make sure you consider an
external audience when writing tasks or comments.

### Pivotal Tracker stages in real life

|      STATE    |  REQUIREMENTS FOR ENTERING STATE |  REAL LIFE ACTIONS |
| ------------- |:--------------------------------:| ------------------:|
| STARTED       | The task has been assigned to you or you have picked it from top of priority list and you are now available to start working on it. You understand what needs to be done and you have all the data / assets / copy required to complete the task. If there are missing resources that you need, don’t forget to notify the relevant person (it might be a data scientist, a designer, or a developer). | You created a new branch. |
| FINISHED      | You have completed the task and it is now ready for review, which means you have written the code, tested the code, written automated tests, seen the automated test build pass, run a codestyle check and fixed any violations before passing it on to a reviewer. | You have created a pull request, written a description of what this is for and how to test this, waited for any automated build tools to pass and assigned 2 reviewers (please refer to code review guide). Please ensure the PR contains the minimum set of changes needed to satisfy the requirements of the PT task, keep it small. |
| DELIVERED     | The reviewer has checked the code for smells, inconsistencies, violations of project-wide conventions as well as tested the code. Testing the code is not required in case of a reviewer who is not on the project team. | The reviewer approved the pull request (please refer to code review guide). |
|               | Code is merged into the integration branch. | 2 scenarios for this:
1. as the code author you merge the code. It is your responsibility to resolve any conflicts, wait for automated builds to pass on the integration branch & resolve any unexpected issues.
2. the reviewer merges the code. This is a quicker flow which does not require a round-trip to the author, and is probably more appropriate for small changes on non-conflicted branches with small potential for regressions. |
|               | Task is ready to test in a non-local environment. Most typically this will be a staging environment. | An automated deploy hook is recommended for deploys from integration branch (develop -> staging). If the automated deploy is not enabled, whoever merged the code should deploy it and verify it is actually ready for testing on the dedicated environment. |
| ACCEPTED      | Task has been verified to work in the testing environment and meet acceptance criteria. Acceptance can be done on the Retrospective/Planning meeting or when the Project Manager reviews the status of Pivotal Tracker | Once all tasks in a release have been accepted, changes from the integration branch can be merged into the production branch. It helps to keep releases small. Here's a useful [branching workflow](http://nvie.com/posts/a-successful-git-branching-model/). |

For designers, data folks and others the Pull Request might not be the
delivery system, but Pivotal Tracker can still be used.

### Planning sprints

The best way to ensure that Pivotal Tracker is up to date is to ensure that
everyone is using it and that it reflects the state of the project.

It is recommended that each project team meets at least once a week to plan
their project sprints. Recommended agenda for such a meeting is:

- Retrospective on previous sprint [if no specific meeting for it], goal is to
check where the project is and if there were any issues;
- Discussion of priorities, the Project Manager should make sure to
communicate any priorities discussed with the client;
- Identification of tasks to work on the new sprint;
- Ensure that all tasks have been estimated;
- Create a release on Pivotal Tracker with the date of the end of the sprint
and describe the goals of the sprint on the description.

After the planning meeting everyone should know what they are working on and
what are the goals for the sprint.

### Tips and Best practices

- Stories and epics have more than a title, you should make sure to read their
descriptions when picking up new tasks, to make sure you know as much as
possible when starting to work on something;
- You can click in your name or in My Work to get a list of the things that
are assigned to you;
- If you find something that needs doing and you can't find an associated
story on Pivotal Tracker, make sure to add it and to explain why it is needed
the best you can;
- Tags help organize work and can be useful to decide on what to work next, if
you're adding new stories make sure to tag them consistently;
- Sprint planning is a team job, everyone should be involved and participate
actively in it; that is the only way that an accurate list of tasks can be set
for a given sprint;
- Don't forget to update your stories when you finish some stage;
- When creating a Pull Request you can add a link to a Pivotal Tracker story
to make it easier for the reviewers to understand what they are reviewing;
- Most of our Pivotal Tracker projects are connected to a channel on Slack, if
you add your Pivotal Tracker handle to your notification list on Slack you
will never miss a relevant message;

### Epics, stories, backlog, icebox, and points

We all know that Pivotal Tracker is a bit complex, below is information on how
the key components could be used successfully.

#### Epics

These are the highest level units on Pivotal Tracker. Epics work well to
organize smaller tasks in terms of a User Story (high level functionality that
the application should support) or a specific website page (when separation in
pages makes sense).

The best way to make use of Epics is to add them at the start of a project and
then use them to tag specific stories. This will allow everyone in the project
to have a sense of what's left to do in regards to each user story.

The Epic's description can hold the full user story or a link to a document
that clearly describes the epic for further information.

#### Stories

Each story represents a feature on the application. Each story should be
clearly labelled with the epic that it's related with and any other tags that
make sense. Stories should also be estimated and if a story doesn't fit in the
points range being used, it should probably be split into smaller tasks.

For further clarity make sure to use the story description to add any detail
or advice that might be relevant. If there are clear sub-tasks on a story you
can also use them to better communicate what's happening with it.

#### Backlog

Usage varies but it seems to work well if we keep only the stories that we are
aiming to tackle in a given sprint, this way there's less clutter and it's
easier to check the pulse of a sprint.

#### Icebox

Here we keep the tasks that are not part of the current sprint but that should
be considered next. It's recommended that the icebox be filled as soon as
there's information about specific user stories, so that there's a pool of
stories to work from.

#### Points

It's recommended to use points as number of hours. A custom range can be set,
and at team Rosling we have been using 0,1,2,3,4,6,8,10,12,14,16. Points
should be set by the team on each sprint planning or after any estimation
effort; they will help define each sprint.

# Warnings

## Avoid spreadsheets and other information sinks

One of the major threats when running a project is that information gets
spread across different tools and not in a central location. Often times
clients will provide a spreadsheet or send a document or information via
email. It is important to avoid using those documents as the information
source as not everyone will have access to them or they will be hard to
maintain. If the client sends one document like that and you can’t convince
them to use Basecamp or Pivotal Tracker (in the cases where clients are also
using Pivotal), you should still add the tasks to the right task management
software yourself. This requires some extra leg work of keeping things in sync
but will benefit the whole team, as everyone will know where to check what’s
happening in the project and what feedback has been
received.

## Avoid private conversations on important project topics

It is normal to have private or even offline conversations about different
aspects of a project be it at high level or more task level. This is normal,
but it is important that all key decisions or comments that benefit everyone
involved in the project be communicated on the project channel. So if you are
having such a conversation assess if it should just happen in the channel for
everyone involved to be able to benefit and contribute to it, and if you still
go ahead and have it in private make sure to communicate back to the channel
the outcomes of said meeting/conversation.

## Assess the impact of client dependencies on our work

One risk of working so closely with our clients is that we depend not only on
their feedback but also on them providing datasets and style guides or other
materials. We should be careful to always define deadlines for the client to
provide us anything that we need from them, and when to decide on what to do
if a deadline is missed. One option is to shift focus to other parts of the
project that are not dependent on their immediate input, but it should also be
considered the possibility of halting development until the input is received.
This should be clearly communicated to the client early on, so that this risk
is well understood.

