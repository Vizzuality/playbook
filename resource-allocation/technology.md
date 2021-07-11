# Technology

There's certain aspects of resource allocation that involve the technology we use as tools, how we experiment and learn new things, and the standards and processes we set for as a company.
This document will hold some common practices and try to centralise and expedite the decision making regarding these aspects.

## How organise a project
Currently we divide project organisation in 3 levels:

### Comunication
Comunication can be divided into two types: internal communication and client communication. For internal comms we use the following tools:
- **Team Slack.** Generally creating a project channel for all the team members to join, and a project dev channel to include the slack integrations with other tools and to discuss stuff concerning development implementations only.
- **Team – Client Slack.** Sometimes when communication with the client is constant, and needs to be more direct, we set up either a shared Slack workspace or a shared slack channel. It's important to note that a shared slack channel is better at avoiding context switching and easier to set up, so we should try to use shared channels whenever is possible.
- **Basecamp.** Used as a way to communicate with clients, this is very helpful in avoiding the loss of knowledge across email threads.
### Issue tracking
- **Pivotal tracker.** Most projects issue tracking is handled using Pivotal Tracker. This tools helps set up the features, bugs and releases of a project sprint.
- **Basecamp.** Although it's mainly used as a way to comunicate with clients, sometimes clients use it to report bugs and track issues.
- **Github Issues.** Used sometimes to track features, bugs and releases in some projects. We should use this in projects where being transparent to the open source community is a priority (i.e. `wri-api-components`, `layer-manager`).
### Version control
- **Github.** We use it as our version control platform. The main approach is to create a repository for each project we have. However when a project has a component-kit that shares with related projects, this component-kit usually is allocated in a new repository.

## Use and research of new technologies and libraries.
As of now we try to use tools that we know have solved the problem we're facing in the past. When we don't have experience with solving a determinated problem, the first thing we do is reach out to our project team, then reach out to the company via slack using a domain specific channel. When we have exhausted our options, and a complete solution hasn't been identified we proceed to research and find a new technology that will solve our needs.

## Processes and Architecture definition
**TODO**

## Supported platforms as a company (AKA do we really want to maintain IE11?)

## Experimentation and research labs
**TBD**
