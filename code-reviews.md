# Code Reviews

Performing good code reviews is a must to maintain the quality of a software project. After a contributor finished a
ticket and makes a pull request to get his work to the main branch, the proposed code changes needs to be reviewed
carefully. Potential bugs, wrong implementations of ticket requirements, mistakes, missing tests, etc. can all be caught
before it's merged.

It also forces contributors to do their best on writing readable, quality and robust code, because he knows that it will
be reviewed by other developers.

## Code reviews are required

Before any code can go to production, it **must** be reviewed by at least one developer. The minimum amount of reviews
is variable and is different per project. It may be two for example.

It's also important to think about the expertise of the reviewers. Do they have enough authority, experience, knowledge,
etc. to determine if a pull request is ready to go to production. This is something that you always to take into
account.

## Universal checklist

The exact code review checklist is different per project. The checklist below is therefore made as generic as possible.

Important aspects to think about while reviewing:

* Implementation
* Security and Data Privacy
* Risk
* Ethics and Morality
* Usability and Accessibility
* Testing and Testability
* Dependencies
* Performance
* Readability
* Experts Opinion

See [this blog post](https://www.michaelagreiler.com/code-review-checklist-2/) with extra information about these
aspects.

## Sources

1. [A Code Review Checklist – Focus on the Important Issues](https://www.michaelagreiler.com/code-review-checklist-2/)