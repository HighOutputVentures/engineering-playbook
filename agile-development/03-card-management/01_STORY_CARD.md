# STORY CARD

## What is a Story / User Story?
A story is a behaviour or feature that a solution needs to implement in order to fulfill the needs of a user.

## Why should we create a Story?
- Stories keep focus on the user
- Stories enable collaboration
- Stories drive creative solutions
- Stories create momentum

## Naming title guidelines
Make it declarative

Creator announces profile to Bitclout

## Writing a description guidelines
As as `<persona>`, I `<want to>`, `<so that>`.

For example:

As a Creator, I want to announce my newly created profile to Bitclout, so that they are aware I signed up on Jamclout.

###  Acceptance Criteria
Gherkin syntax

By using this syntax `GIVEN`, `WHEN` and `THEN`.

For example:

```gherkin
GIVEN the request have the status PENDING
WHEN the admin tries to approve it
THEN it should return an error
```
## Resources
1. https://www.atlassian.com/agile/project-management/user-stories
2. https://stratejos.ai/blog/naming-task-bug-user-story-titles/