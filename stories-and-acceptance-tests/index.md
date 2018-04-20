# **Job Stories and Acceptance Tests.**

# Intro.

This document explains how Vizzuality uses Job Stories and Acceptance Tests to finalise project scope with our clients and deliver quality products. We will talk about three key elements:

* User Personas: a brief description of a key audience group that we want to target in a certain project.

* Job stories: a series of statements that describe specific interactions users will want to complete on the interface, and why. The ‘why’ is made up of the original context for visiting + what they’ll want to achieve afterwards. 

* Acceptance Tests: a series of scenarios describing how a tool may be used, so we can check it solves the problem we want to solve with the tool. They go into more detail about the scenario of the user. 

Each of these activities should be completed with the core project team, with responsibility for coordination and delivery attached to the Project Manager and User Researcher.

# Start with the Persona.

One of the first activities we do on any project is to ask "who is the target audience, and what do you want them to do on the tool". We usually summarise these discussions in a user persona document. Personas are ‘stereotypes’, representing the average user within a group. Usually we would focus on around 3 priority user groups: adding too many more means we could lose focus and compromise the user experience. 

Each persona should contain the following information:

* Name of persona

* Type of Organisation they work for/ sector they work in

* Seniority/ Job title

* Level of experience with the internet

* Level of experience with data visualisations

* Their responsibilities/ what do they do in a normal day?

* What barriers do they face to achieve their goals?

* Desires/ Needs: What will they want from the tool we build?

* How will they hear about the tool?

* How often will they use it? 

[There’s a template in the Google Docs gallery](https://docs.google.com/document/u/0/?tgif=d&ftv=1) that you can use to undertake this activity. 

Examples from our projects: 

* [Mozilla](https://docs.google.com/a/vizzuality.com/document/d/1nrx25Cn59ZIGFJCMV5NRhupypwKBkn_12O_zIRZbSB0/edit?usp=drive_web)

* [This presentation for Radiant](https://docs.google.com/a/vizzuality.com/presentation/d/1kwh9aDGXfbf8lBf9S9c4I4ebKNdmVZmPGq1BRe2pISk/edit?usp=drive_web)

* [This work for Climate Watch](https://docs.google.com/presentation/d/1BMxoVtx54c0MYwCcIvxb0Z3ngJFHwoLRpGnmePMYNvg/edit#slide=id.p)

* [Wilmap (this one was done with the client)](https://docs.google.com/document/d/1J-nIxMMlmU4o2uEAiKyGGLVYMKJjeGKfJ8z4aw5A_GQ/edit#heading=h.te9kz0fedbzu)

# Then write Job Stories.

Job stories are specific statements detailing which problems users want to solve using the  interface. We use Job Stories to drive conversations about what could be put on the site, and to make sure we create a number of solutions that will deliver real value to users. Our solution is ‘successful’ if it helps users complete these stories quickly and easily. Following these discussions we would refine the stories into a final list, which can be used to start writing acceptance tests (see below). 

Each statement contains three parts:

* "When I"...   - the Situation/ Trigger, why is the user coming to the tool? 

* "I want to"...    - Motivation: what are they trying to do on the tool? 

* "In order to".    - Objective/ outcome: what do they want to do once they’ve successfully used the tool?

Job stories should be written in the middle of discovery, once we have enough information about who may use the tool, what users want to try and do, the data and client expectations. Some guidelines include:

* Single Responsibility Principle: you should express only one problem in one story. 

* Written from the viewpoint of a user: if we gave the list of stories to a user, they would understand them. 

* Focus on problems: stories should not prescribe a specific functionality (user can see a graph) but a problem the user is trying to solve (I want to see change over time).

* Focus on Context: make sure you’re explaining why a user is coming to the site, what they’re trying to achieve and what comes next after they use the site. 

* Prioritise: share the stories with the client and complete a prioritisation exercise, to establish which stories are most important for us to work on.

The job stories can then be used throughout the project in discussions about project scope or comments on prototypes and design drafts. 

Examples:

*When I’m* writing a national report on the state of the environment, *I want to* find out the current status and change since 2010 for biodiversity indicators for my country, *in order to* complete the report faster and fill gaps in the data I have. 

*When I’m* writing a soy sustainability strategy for my company, *I want to* see how much of the soy we purchase comes from areas with low sustainability,* in order to *eliminate them from our supply chain. 

*When I’m* writing a 10 year strategy about water stress for my company, *I want to* see if any basins we rely on will suffer severe water stress in the next 10 years, *in order to* create plans to support growers in those regions and guarantee the supply of commodities into the future. 

Examples from our projects

* [Aqueduct](https://docs.google.com/document/d/1taUfuvXu4pacDE0TBf8g1bFo-xORddXqQcgmL6oK2xM/edit#heading=h.x2vydgfott77)

* [R4D nutrition project](https://docs.google.com/document/d/154RndawLKyVsp3yhRpS10jF0i9IaVlCF03UqOZam9rg/edit)

# And finally, Acceptance Tests.

Acceptance tests break down the job stories into even more constituent parts, providing clear statements about what interactions a user can complete on the interface. We should also cover things like cross-browser compatibility and mobile responsiveness here too; [examples of these kind of statement here](https://docs.google.com/document/d/1QuF1M7k6VtBEtkHyQFvriQp1qi-aiKu1zrjB3pHoxB0/edit#heading=h.edug73oecu7z). These statements can then be used to form a test script (in conjunction with the kinds of scenario depicted in Job Stories), or to define whether a feature has been completed. 

Example:

For the first job story described in the previous section, acceptance tests would be:

* User can scroll through a list of countries on a landing page. Hovering over a country would highlight it. Clicking a country takes them to that page. 

* User can scroll through a number of indicator widgets, by default showing the latest data

* User can click a button to see the change since 2010 in each widget

* User can click a download button on each widget. This will trigger the download of a csv of the data for that widget. 

* User can find a citation for the data in a modal by clicking an information icon

* User can view the page on IE9

* User can view a non-interactive, responsive version of each widget when accessing through a mobile browser. 

Examples from our projects:

* [Trase](https://docs.google.com/document/d/1kRkIqmlZlTqIMq8cyX1fgAGmKvKqHzIw5nVOSyznwT0/edit)?

* [Climate Watch](https://docs.google.com/document/d/1ScvbpOhl0h0XB54KEdOtb_yX4nTJg9q6Y4YoIB27Slc/edit) (note the acceptance tests are still fairly high level)

* [Mozilla](https://docs.google.com/document/d/1XaBjsa2DT1CTbxPb977mKPrxVYrTLc0uGXEH_BLBAKY/edit#heading=h.5d44p4h1pty4)

* [Resource Watch](https://docs.google.com/spreadsheets/d/1amfWhi6vPewo9w5P6kNxDyL35Air0Br_Qyee9tjSO4A/edit#gid=0) (note these tests are much more specific + have a flow)

