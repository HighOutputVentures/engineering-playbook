# STORY CARD

## What is a Story / User Story?
A story is a behaviour or feature that a solution needs to implement in order to fulfill the needs of a user.

## Why should we create a Story?
1. It keeps focus on the user.
2. It enables collaboration.
3. It drives creative solutions.
4. It creates momentum.

## Naming title guidelines
Make the title _declarative_<sup>[1](https://github.com/HighOutputVentures/engineering-playbook/blob/main/agile-development/03-card-management/01_STORY_CARD.md#terms)</sup>.

For example:

Creator announces profile to Bitclout

## Writing a description guidelines
As as `<persona>`, I `<want to>`, `<so that>`.

For example:

```
As a Creator, I want to announce my newly created profile to Bitclout, so that they are aware I signed up on Jamclout.
```

###  Acceptance Criteria
Make use of `Gherkin`'s syntax by using `GIVEN`, `WHEN`, `THEN` and many more.

For example:

```gherkin
GIVEN the request have the status PENDING
WHEN the admin tries to approve it
THEN it should return an error
```

## Terms

1. It consists of a subject and a predicate. 

        For example:
        
        My patient is having a hard time.
        
        The sky is blue.
        
        User is frustrated.

## Resources
1. https://www.atlassian.com/agile/project-management/user-stories
2. https://stratejos.ai/blog/naming-task-bug-user-story-titles/