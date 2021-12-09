---
layout: default
title: Branching model
nav_order: 2
---

# Branching model

Git is a great tool to track changes made to a code base. It makes working in the same code base a breeze. While there is usually a similar flow of how code changes are going to the main branch, there are a lot of different branching models. The most popular is for example Git Flow, but GitHub Flow, GitLab Flow and One Flow are also available. These flows are usually modified to conform the situation.

There different type of repositories. Some repositories contain an application that will be deployed to at least a production environment and probably some test and sandbox environments as well. These type of repositories have a different need than for example packages, developer tools or documentation buckets. Below are these types defined:
* Application
  * Has a deployment process with different available environments. Can follow the SemVer version scheme.
* Package
  * Needs to follow SemVer when being released to package ecosystems.
* Development tools
  * Can vary in many ways

## Application

Repositories that contain an application (web, mobile, service, etc.) will have at least two branches:

* `production`: This branch contains the version of the application that's currently live and in use in production. Based on this version an artefact will be created that will be deployed to the production servers.
* `acceptance`: This branch will be used to test new features, bug fixes, etc. before it goes to production.

The acceptance branch should always be production ready. That means it should not be used to test code on the environment. When the product owner / project manager approves a ticket after testing it on the acceptance environment, we should be able to deploy it to production without a high potential of breaking changes.

Branch naming convention when working on tickets:

* **feature/<ticket-number>-<short-feature-description>:** When the ticket is about introducing a new feature.
* **bugfix/<ticket-number>-<short-bugfix-description>:** When the code change fixes a bug.
* **hotfix/<ticket-number>-<short-hotfix-description>:** When something is broken on production and should immediately be fixed. This can go straight to the `production` branch.

Always include a ticket number in the branch name, this will make it easy to find the corresponding ticket.

All work branches in base should branch off from the `producion` branch to make branches independent of each other, meaning they will not block each other. Working branches can also branch of from other ticket branches, when they dependent on each other. Tickets can be quite big sometimes and can depend on many other tickets. In this case the developers needs to come up with a smart strategy to solve this. A solution could be to branch of from someone else's branch and merge back into the parent once it's reviewed and done. This will create a chain of branches. Another option is to create one big branch where multiple developers merge to. This can be used for Epics for example.

Once you're done with your ticket you should create a pull request to the `acceptance` branch and wait till the minimum amount of reviews has been given. The given reviews should also be according to the [code review guidelines](code-review-guideliens.md). Make sure that the builds are not failing.
