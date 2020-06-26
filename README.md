## Written submission

Please provide written answers to / explanations on the following topics.

Make a PR with your submission to this repository.

## Product/System features

Please explain the steps you think are necessary to perform to get a feature done, from an idea to an implemented solution that is running in production. Be as detailed as possible.

## Scrum vs Kanban

Please explain the major differences between the named Agile frameworks. Which one did we practice during the bootcamp? Can you see any arguments for using a different framework in a specific project or projects?

## Continuous Integration

Explain what continuous integration is and what benefits you can see it brings for teams development workflow. Please refer to your own experience.

## Automated tests

What are the various types of testing strategies covered under automated testing? What benefits do each of them bring to the table?

---

### Product/System features

#### Plan Phase:

First,dev team should draw out a user story about the feature aforementioned. They need to discuss in detail how the feature will be presented to user and how it will work. Lo-fi's will be ver helpful for visualiztion of the feature and will be a guide during implementation.
If the feature can be divided into other features it must be divided because a feature is a small increment of improvement to the project. And if a feature seem not to effect user experience or effect very little. It can be classified as a chore or bug respectively, there are not treated as features.

Secondly, team must discuss together what acceptance criterias are and note them down as bullet points, Everyone must understand these steps and know the feature's impelementation is finished when all of the acceptance criterias are fulfilled.

Lastly, team should vote on how much effort should be required to finish the feature. Each team member must express why it should take too much effort/time or too little effort/time depending on their votes. these vote ratings will be used to calculate the team's progress in sprints so that team can know how much they can handle during one sprint.

#### Coding Phase:

The person or people who are responsible of the implementation of this feature should get the latest development branch from version control and start off a branch from there. To avoid confusion between team members, the branch name must be descriptive.

After branching off, it is better to create pull request on main repo development branch right away, Putting WIP in front of the pull request will prevent confusion and will provide info what it being worked on.

Before writing the actual code happy and sad paths must be considered and tests should be written accordingly. Running tests and fixing each error one by one will guide us to write our code and prevent us to wander off the scope of the feature. If something is not required to pass a test, then dont do it. This will keep the implementation code less comples and on point to the feature. It would be good a practice to commit often whenever a test example is passes.

When implementation is finished, pull request on the main repo development branch must be explained in detail and contain link to the feature's Pivotal Tracker.

#### Review phase

Once developer thinks pull request is ready, he/she should notify responsible person and team members to review it.
Developer must be ready to reply to their comment and do changes if needed.

### Continuous Integration

Continuous integration is a development practice that requires developers to integrate code into a version control repo several times during implementation progress. Each pull request is then verified by an automated build,allowing teams to detect problems early. By integrating regularly
you can detect errors quickly and locate them easily.
Since we are integrating regularly, there is less back-tracking to find the problems in the code. A rule of thumb if the tests are not passing, do not merge it. Keeping the development branch passing all tests helped us to build add features on top each other without breaking other parts of the application. CI does not eliminate bugs totally but it makes it easier to find and fix them. But whenever we pulled from our development branches that this version of our app is working and tests are passing. So we know that whatever we do on our feature implementation will be the cause of bugs and not passing tests. We are always handed a working application from development branch with CI

### Automated Tests

#### Unit/Model/Component/Integration Tests

    Unit tests are written from developers perspective, they are made to ensure that a particular method/controller/model or component performs
    a set of specific tasks correctly. They are tested in isolation, but when relationship between two units are being tested, this kind of test is called integration testing. Another way to look at integration test is making sure units/models working together as a whole. With unit/models tests you can test edge cases of your units.

#### Accceptance/E2E/Feature Tests

    With Acceptance,E2E and Feature tests, developer tests the application by interacting with it just like a real user would do, since this combines many parts of code base, this is also an integration test. This type of testing is driven by Behaviour Driven Development, you design your test as how a user would your application. You are making sure the application is not broken in a such way that a user might notice.

### Scrum vs Kanban

Kanban is a task oriented management flow, where taks are prioritized in a queue and worked on until they'r done. It's very well suited to manufacturing and IT or any group that does as-needed work.
Scrum is a story/goal oriented workflow focused on the needs of end users as determined by product owners in the business. Large scale user-stories are broken down into discrete pieces of work then completed.
The biggest difference between the two is that Scrum is tailored to estimating and working on large-scale projects by completing small quantities of useful work that eventually completes a bigger picture idea for the business while Kanban is about fixing specific issues or doing specific work that are themselves the goal.

We practiced Scrum in our projects, but I can tell that Bugfixing and Chores during our projects can be done using Kanban because It focuses on getting the most important thing done as quickly as possible and moving things to done. I believe Kanban will make us move faster among bugs and other non-user scoped related issues.
