# How to allocate and manage cloud resources

This guideline covers the steps you should take should you need a cloud resource, like a server to host a project, a file bucket, a Carto/(something else) account, etc.

## Project resources

Most of our projects require some sort of hosting to run on, be it a server to run code on, some hosting-as-a-service like Heroku, and S3 bucket to store files etc. More complex projects may need certain services, like Carto, Google Earth Engine, Transifex, etc.

### Resources owned by the client

While there are multiple ways in which these resources can be provisioned, the recommended way is to talk with the client and have them own these resources themselves. This carries a series of advantages both to us and the client:

- If they own their resources, there's no transfer cost or delay for either us or them, should they decide to hire another provider in the future.
- They own the service accounts, much like they own the code/design/etc we build for them.
- Should they already have a cloud infrastructure, they can consolidate to cut costs.
- For the duration of the project, we are available to have technical ownership of these resources, so we'll still set up resources as needed, even though they are not owned by us.
- Billing is handled directly between the client and the service provider, without us being needlessly in-between the two. 


We should be clear and transparent when communicating the need for these resources with the client, as these costs can appear as unexpected to some clients, and their internal budget for the project may be restricted:
- We should discuss with the client why this resource is needed.
- We should, when possible, present alternative solutions to the problem, and provide a recommendation based on our expertise, as to why a given solution is superior to the others.
- We should provide an estimated cost of the service, identifying what are predictable costs (ie: VPS costs are fairly easy to predict and vary very little) and what is harder to predict (ie: network traffic cost is often hard to predict). Clarify that it will be charged by a 3rd party, over which we have no control. Useful links:
  - [AWS calculator](https://calculator.s3.amazonaws.com/index.html)
  - [GCP calculator](https://cloud.google.com/products/calculator)
  - Google: "<name of the tool or service> pricing"
- We should be upfront about the cost of these resources.
- We should clarify if the cost is temporary (ie: staging servers) or "permanent" (ie: production servers).
- Whenever we make a change that modifies these costs, we should tell the client beforehand.


Given that setting up these resources can be a quite technical process, we can help the client with the practical steps, by:
- Creating the necessary service accounts for the client, using their data.
- Setting up the resources for them.
- Providing links or other resources that helps them carry out the process themselves, should they wish to.
- Joining them on a call, screenshare, and guide them step by step if they prefer to do these steps themselves.
- Provide links or other resources covering any post-delivery maintenance tasks they may need to carry out (or advise them to hire external help, should you think that's the best option for them).

During this, we should use and recommend to clients our [security best practices](https://github.com/Vizzuality/playbook/blob/master/guidelines/security.md) when it comes to picking passwords, sharing and storing them, etc. 

Once the development phase of the project is over, don't forget to backup and delete any staging resources that may have costs associated, so we keep our client's bills as low as possible.

#### How to handle credentials for client owned accounts

Once resources are provisioned, you should save any and all credentials to Lastpass, and share them with the team members that may need access to them. Do not keep these on your Lastpass account only, as this exposes the team to [the bus factor](https://en.wikipedia.org/wiki/Bus_factor). Additionally, some credentials are only available when created, so if you don't save them straight away, you may need to regenerate them, which means updating servers, etc.

Once the project is over, and if we are not anticipating any further work, we should recommend that the client resets passwords, so they have exclusive access to their accounts.


### When "we" are the client

For some projects, we are our own client (for example, grant-based projects), so the above doesn't apply. For those situations, Vizzuality has its own set of accounts on Google, AWS, etc, that we can use to host and support our own projects, keeping in mind the following:
- First of all, you need to check with the PM if it's ok to allocate these resources to the project. The PM should check what the contract says about this type os costs, and decide how to proceed. 
- Our accounts can have resources allocated to multiple projects, so be sure to name and/or tag the resource in a way that makes it easy to match it to its corresponding project.
- For the same reason, clearly identify if a resource is a staging resource, and can be deleted once the development phase is over.
- On the project documentation, clearly identify these dependencies on external services, should we need to make adjustments in the future (ie: renew api keys, migrate accounts, account spring cleaning, etc). 
- Talk with the PM so the cost of these resources can be accounted for.


#### How to handle credentials for our accounts

Once resources are provisioned, you should save any and all credentials to Lastpass. Given that Vizzuality accounts will be needed for longer than the duration of a single project, you should check if the particular platform you are using supports having different user accounts per person. If it does, take your time to set up your own account, instead of using someone else's. Be sure to follow the [security best practices](https://github.com/Vizzuality/playbook/blob/master/guidelines/security.md) when it comes to things like password strength, storage and 2 factor authentication.

If you are creating a new account on a new service, or if the service does not allow or have more than one set of access credentials, be sure to store the credentials on Lastpass, so we are less exposed to [the bus factor](https://en.wikipedia.org/wiki/Bus_factor). Additionally, some credentials are only available when created, so if you don't save them straight away, you may need to regenerate them, which means updating servers, etc.

When setting up a new login for a colleague, you may need to define roles and permissions. When doing so, talk with them about which tasks they will be carrying out, and grant them the minimum needed permissions to carry out those tasks. Hacks happen, so the less permissions an account has, the less damage is done in case its compromised. 
