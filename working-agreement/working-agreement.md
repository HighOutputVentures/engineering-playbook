# Working Agreement

## Working Agreement

A working agreement is a document that describes how we work together as a team and what our expectations and principles are.

### General

* We work as one team towards a common goal and clear scope
* We make sure everyone's voice is heard, listened to

### Communication

* We add all documentation to the project repository

### Backlog Management

* We follow the Definition of Ready when we move it to `To Do`
* We make our work visible through work
* We assign ourselves a task when we are ready to work for it. and move it to `In Progress`
* We follow the Definition of Done when closing cards
* If add a sub-task card, we make sure it matches the acceptance criteria of the user story, to avoid scope creep.

### Code Management

*   We follow the git flow's naming of branches

    For example:

    `feature/add-add-user-api-endpoint`
* We merge through PRs
* We treat documentation as code and apply the same standards

## Definition of Ready

When the development team picks a user story from the top of the backlog, the user story needs to have enough detail to estimate the work needed to complete the story within the sprint. If it has enough detail to estimate, it is Ready to be developed.

> **💡 Advisory Note:**
>
> If a user story is not Ready in the beginning of the Sprint it increases the chance that the story will not be done at the end of this sprint.

To help team members to ensure that the user story they wrote contains all the necessary details for the scrum team to understand the work to be done.

* [ ] \- Does the user story have clear and complete acceptance criteria?
* [ ] \- Does the user story address the business needs?
* [ ] \- Is the user story small enough to be implemented in a short amount of time, but large enough to provide value to the customer?
* [ ] \- Is the user story blocked? For example, does it depend on the following:
  * A deliverable provided by another team
  * incomplete work

### When should a Definition of Ready be updated

Update the `Definition of Ready` anytime when the team observes that there is the missing piece of information in the user stories that repeatedly impacts the planning.

### What should be avoided

The `Definition of Ready` the checklist covers items that apply in a general. **Don't add items or details that only apply to one or two user stories**.

### How to get the User Stories Ready

## Definition of Done

Provides a list of example checklists to verify that the user story or release is a success.

### Goals

To help clarify the expectations of all team members and judge if a story is complete or a release has been confirmed as a success.

To close a user story, a milestone, or set for a release it is important to verify that the tasks are complete.

#### User Story

* [ ] \- Acceptance criteria are met
* [ ] \- Refactoring is complete
* [ ] \- Code build without error
* [ ] \- Unit tests are written and pass
* [ ] \- Existing unit tests pass
* [ ] \- Code review is complete
* [ ] \- UX Review is complete (if applicable)
* [ ] \- Documentation is updated

#### Release

* [ ] \- Definition of Done for all user stories included in the sprint are met
* [ ] \- Product backlog is updated
* [ ] \- E2E tests pass
* [ ] \- All bugs are fixed
* [ ] \- Release is marked as ready for production deployment by product owner
