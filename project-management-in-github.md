# Project management in GitHub

<summary>

## Repository Projects

Each repository will have a main GitHub-project called `Project Board` that will be used to manage, maintain and keep track of the repository on a global level. The project needs to be based on te template `Automated kanban with reviews` by GitHub.

This will set up the part of the required columns including a workflow to automate the location of issues and pull request within the columns:

* Backlog (needs to be added manually)
* To do
* In progress
* Review in progress
* Reviewer approved
* Done

## Tickets (issues and pull requests)

Our planned and unplanned work needs to be written down and documented in tickets. This ensures that anyone can go back in time to find out why something was created, what the requirements are, which decisions where made in the process and anything else that might be useful to help that person.

A ticket is nothing more than a collective word for an event that must be investigated or a work item that must be addressed. Within or system the following type of tickets can be created:
* Task
* Bug
* User story
* Epic

To mark an issue or pull request with one of the types, we will be using the label functionality from GitHub. This will allow us to identify these types more easily and filter based on them.

It's important for the maintainability of the repository that **all issues** are given a type. This will be checked by a bot in the future (https://github.com/KA-Huis/space-management/issues/18).

### User story estimations

User stories will be required to contain an estimation once it's moved from the `Backlog` column to `Todo`. This will be assigned using labels as well.

The estimation is not time based, but complexity based. Therefore, we'll be using a slightly modified version of the Fibonacci sequence:
* 1
* 2
* 3
* 5
* 8
* 13
* 20
* 40

### Priorities

There is usually a difference in the priority of tickets. There a few level of priorities that can be assigned to tickets. This will help with identifying high priority work from less important work.

* Highest
* High
* Medium
* Low

### Standardised labels including color

#### Ticket types

| Name | Description | HEX color code |
|------|-------------|----------------|
| Task | Something needs to be done | #0251E6 |
| Bug | Something isn't working | #d73a4a |
| User Story | | #0D742E |
| Epic | | ##B55CEF |

#### User story estimations

| Name | Description | HEX color code |
|------|-------------|----------------|
| Estimation: 1 | | #674C37
| Estimation: 2 | | #674C37
| Estimation: 3 | | #674C37
| Estimation: 5 | | #674C37
| Estimation: 8 | | #674C37
| Estimation: 13 | | #674C37
| Estimation: 20 | | #674C37
| Estimation: 40 | | #674C37

### Priority levels

| Name | Description | HEX color code |
|------|-------------|----------------|
| Priority: Highest | | #750C27
| Priority: High | | #750C27
| Priority: Medium | | #750C27
| Priority: Low | | #750C27