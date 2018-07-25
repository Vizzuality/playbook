# Quality checklist
We want a minimum check to be applied to different aspects of the project to ensure that the end-product meet our high standards. We have identified several key criteria to check in four broad areas of a project's life cycle. 

## Research
There are a number of discovery activities included in the [main Project workflow](https://docs.google.com/document/d/1MGC8xPRhHqr7SbqFHh2k0Bmqo_4eyT2M3WzD8AjCBVg/edit), which are broken into smaller steps in the [long version of the Research Workflow](https://docs.google.com/document/d/1AMAnbLkAFG0hIkJIIDID0oBchPIAPIeT1-Rq5x7SnTo/edit). In this document we outline the steps we need to take to ensure a quality delivery of each output. 
1. Consult the [list of research methods](https://docs.google.com/document/d/1HJet_b_4rORsQ5vxi3IDhCWHOVAFlKZpQboa7hKIJ_g/edit#) + project scope - which activities would be suitable? Could we try something new with this project?
2. Discuss scope of the output with the Project Manager, and set a goal for internal delivery. 
Define the boundaries of ‘quality’:  how many users do you need to interview from each user group to have a representative sample, how many survey respondents do you need, what is a representative time period for an analytics review? 
3. Follow the [Personas, Job Stories and Acceptance Test structure](https://vizzuality.github.io/playbook/projects/stories-and-acceptance-tests/) where possible.
4. Share a first draft with Research team for comments.
5. Introduce the output to colleagues in a meeting (PM + design + data + lead engineer) and ask for feedback. 
6. Refine using their comments, and present to client. Again, hold a meeting to present your findings and gain feedback. 
7. Publish a final version on Basecamp and add a link in the Project Template.

### Other Tips
**Write in plain english.** Not all clients will know what a persona is etc. Make sure to present clearly what each output can be used for. Consider using Hemingway to test the readability of your work. 
**Give adequate time for review.** Notify colleagues ahead of time when to expect a draft. Once they have the document, give them enough time to read. 
**Keep reflecting on the research methods doc.** Every project is an opportunity to try a new approach, or refine our existing methodology. After each discovery period the team should reflect on what was achieved, and note down any improvements in that document. 


## Data
While individual projects and datasets may differ significantly, broadly speaking, where possible we should be attempting to ensure the following criteria are met:

1. Aim for open source and open access
Datasets are being held within projects in a way that makes them openly accessible and with licenses that enable their reuse.

2. Keep a clear chain of custody and metadata
We should aim to make the data provenance clear: i.e. document the point of origin, chain of custody and make clear any transformations or pipelines which have been applied to datasets that may have modified their contents. Datasets should also be described with metadata.

3. Encourage dataset reuse across projects
We should avoid siloing datasets and pipelines to individual projects. Datasets (and the knowledge of how to work with them) are resources, ideally we would want to use these resources again in the future. This is particularly important as we have many projects with overlapping spheres of interest. Where possible projects should encourage the use of datasets in a way that builds off of the usability and knowledge of datasets already used in the company, and in turn shares new datasets where possible. 

4. Ensure data transformations and pipelines clear and reproducible
We should at minimum be able to easily understand and replicate any modification to the original datasets, and produce any derivative data generated over the course of a project. Key practices that can ensure this include the use of technology like Docker and Jupyter notebooks.

5. Ensure we are delivering as much value as is reasonably possible
Often, the majority of time can be spent in the preparation and data engineering and bug fixing side of a project’s data tasks. We need to ensure that in addition to that we should make sufficient effort to deliver value beyond simply engineering the datasets into a minimally useable format - we should be aiming to deliver products that derive meaning and insights from raw data.


## Design
- [ ] The researcher reviewed the wireframes/design and gave them a green-light [  ]
- [ ] The developer reviewed the design deliverables before starting implementation
	- UI Kit, Icons (Icomoon), Compressed Images, Interactions...
- [ ] The designer reviewed the implementation and gave it a green-light
- [ ] The designer had big enough / uninterrupted chunks of time to focus on the project
	- Can we create a hard rule? 1 week 1 project?
	- Can development support / meetings happen in fixes hour of the day?
- [ ] Presentations included explanations
+ Add other project-specific quality checks when needed
