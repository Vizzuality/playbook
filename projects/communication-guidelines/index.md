# Project Communication guidelines

## Communication with the Client

Broadly we could think of 4 main needs regarding the channels of communication with the client:
![Communication channels with the client](communication_channels.svg)

### Task Management System
Our recommendation for this is to use [Pivotal Tracker](https://www.pivotaltracker.com/dashboard). Ideally tasks should have meaningful tags/labels associated to them so that filtering by feature/priority/topic... is easier. Besides that they will normally be included in an epic.
We recommend that only one person from the client's side can create tasks -normally the Project Manager, while everyone else from their team should be able to add comments to the tasks. Internally everyone should be able to create tasks, although in many cases the person who would do this would be either the Project Manager or an "area manager" _(frontend, backend, UX, etc)_.

### NRT(Near-Real-Time) communication channel
Slack seems to be a good choice for this. If the project is big/important enough, a dedicated Slack site should be created for it. Having at least the following channels proved to be useful:
* general
* bugs
Perhaps we could add a third one *releases* were we could be posting the progress made on the production site _(we've been using the general channel for this in RW)_

### Discussions or "reference" channel
This refers to the broad discussions that are held before something is defined enough as to create a set of tasks in order to build it. Having this kind of conversations in [Basecamp](https://basecamp.com/) was helpful as it not only served to have the discussions themselves, but also as a reference for the conclusions and decisions made for general topics along the definition/implementation process.
Normally a new thread would be open for each topic and messages would be exchanged there until a conclusion has been reached.

### Admin channel
By Admin channel we mean the tools or ways to define things such as the scope of a contract, budget estimates, etc with the client. So far we haven't used any specific tool or procedure for this but rather exchange Google Cloud documents and spreadsheets. Perhaps it would be worth it to explore better options.

## Internal communication

### NRT(Near-Real-Time) communication channel
We recommend Slack for this, the following set of channels proved to be quite useful in the case of RW:
* Dedicated channel _(e.g. #resourcewatch)_
* Dev channel: _(e.g. #resourcewatch-dev)_: Including a hook to Pivotal Tracker using [Zapier](https://zapier.com/apps/pivotal-tracker/integrations/slack)
* Jenkins channel _(e.g. #resourcewatch-jenkins)_: Including a hook to Jenkins notifications.
