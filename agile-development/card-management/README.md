# Card Management

## Overview

Add guidelines and lean processes on different issue types, columns, and swimlanes to easily track meaningful progress.

## EPIC CARD

### Description

Are large bodies of work that can be broken down into a number of smaller tasks (called stories).

### Why should we create it?

To categorize and organize common pieces for the required work into a shippable piece.

### When should we create it?

When there are initiatives or features that can be broken into deliverable pieces.

### Difference between Epic and the other issue types?

Other card issue types describe a single piece of work, while epics on the other, are used to describe a group of issues related to the same, larger body of work.

### Writing the `Title`

Make it shorter and easy to understand, you can initially name it like this.

**Example(s)**

```
- Post

- Notifications

- Member Management
```

> **NOTE**: However, there are some instances that you want to further narrow down the scope to fit on a release cycle

**Example(s)**

```
- Bookmark Post

- View All Read Notifications

- Update Members
```

### Writing a description guidelines

An elevator pitch (value statement) that describes the epic in a clear and concise way.

#### You can follow this kind of format

```markdown
For <customers>
Who <do something>
The <solution>
is a <something - the "how">
that <provides this value>
unlike <competitor, current solution, non-existing solution>
our solution <does something better -- the why?>
```

## STORY CARD

### Description

A story is a behavior or feature that a solution needs to implement in order to fulfill the needs, from the user's perspective.

### Why should we create it?

1. It **keeps focusing on the user**.
2. It **enables collaboration**.
3. It **drives creative solutions**.
4. It **creates momentum**.

### Naming title guidelines

Make the title _declarative_[1](../03-card-management/01\_STORY\_CARD.md#terms).

**Example(s)**

```
Creator announces profile to Bitclout
```

### Writing a description guidelines

Follow this format.

As as `<persona>`, I `<want to>`, `<so that>`.

1. `Persona` - can be an Admin, Creator, Recruiter, Manager.
2. `Want to` - What the persona wants to achieve.
3. `So that` - Why do they need to achieve it.

**Example(s)**

```
As a Creator, I want to announce my newly created profile to Bitclout, so that they are aware I signed up on Jamclout.
```

Add more details to eliminate assumptions.

#### Acceptance Criteria

Make use of `Gherkin`'s syntax by using `GIVEN`, `WHEN`, `THEN` and many more.

1. It should be written in 3rd Person
2. Each step should be declarative
3. Each should define a scenario

**Example(s)**Scenario: PENDING requests cannot be approved immediately

```
GIVEN the request have the status PENDING

WHEN the admin tries to approve it

THEN it should return an error
```

For more details, Acceptance Criteria.

> **⚠️ TAKE NOTE:**
>
> Not all acceptance criteria that is written under the story card are worth to be written in test automation.
>
> For more details see, Writing an E2E tests

### Terms

1.  It consists of a subject and a predicate, For example.

    ```
     My patient is having a hard time.
     
     The sky is blue.
     
     The user is frustrated.
    ```

## TASK CARD

### Description

It is a card, mostly used outside business flow.

### Writing a `Title`

Make the title _imperative_[1](../03-card-management/02\_TASK\_CARD.md#terms).

**Example(s)**

```
Write a migration script for handling hashed value for the field, `bankAccountNumber`.
```

### Writing a description guidelines

It should define the purpose and the additional details for this task.

### Terms

1.  It expresses direct command, For example:

    ```
     Commit the message.

     Delete the row.

     Please join us for dinner.
    ```

## BUG CARD

### Description

It is a problem that impairs a product or a service's functionality.

### Naming title guidelines

Naming the title for a bug card should help developers point out a specific problem.

We can format the bug card, like these:

1. `<persona / type of user>` `<contraction>` `<perform action>`
2. `<system feature> should <expected behavior> but doesn't`
3. `<persona / type of user> <gets result> but should <get different result>`

> **NOTE**: There are several ways to format the title of a Bug card.
>
> Please see [Naming Bug Cards](https://stratejos.ai/blog/naming-task-bug-user-story-titles/)

**Example(s)**

```
New user can't view homescreen


Member should not be able to see the other member's status.
```

### Writing a description guidelines

Add more details to guide the developer(s), like screenshots and narrowing down scenarios.

**Example(s)**

The new users can't view the home screen when certain events



Add actual results and the expected result.

## HOTFIX CARD

### Description

Unlike bug cards, this card should be tested solely by developers who fixed this and bypassed the QA-related pipelines before releasing it to production.

### Naming title guidelines

Example(s)

`New user can't view homescreen`

> **NOTE**: There are several ways to format the title of a Hotfix card.
>
> Please see [Naming Hotfix Cards](https://stratejos.ai/blog/naming-task-bug-user-story-titles/)

### Writing a description guidelines

Add more details to guide the developer(s), like screenshots and narrowing down scenarios.

**Example(s)**

`New user can't view homescreen when certain events`

## SUB-TASK CARD

### Description

This is to further break down Story Cards into a fine-grained unit of work. This also serves as a guide for developers.

### Naming title guidelines

Make the title _imperative_[1](../03-card-management/02\_SUB\_TASK\_CARD.md#terms).

Example(s)

`Add an GraphQL endpoint to update a pending item`

### Writing a description guidelines

It should define the purpose and the additional details for this task.

**Example(s)**

`The item can be updated when the field, status, is PENDING.`

`The update would return an error message if the status is not PENDING.`

## ISSUE CARD

### Description

This is a bug card under a specified story card. This can help us limit the scope of the incident

### Naming title guidelines

**Example(s)**

`New user can't view homescreen`

> **NOTE**: There are several ways to format the title of a Issue card.
>
> Please see [Naming Bug Cards](https://stratejos.ai/blog/naming-task-bug-user-story-titles/)

### Writing a description guidelines

Add more details to guide the developer(s), like screenshots and narrowing down scenarios.

**Example(s)**

`New user can't view homescreen`

## Board Columns

### Example

### To Do

These are priority cards moved from the Backlog and ready for development.

### In Progress

These are cards that are ongoing.

### Ready For QA

These are cards ready to be tested.

### QA In Progress

These are the ones that are being tested.

### QA Failed

These are the cards that failed on testing.

### Done

These are cards that passed the testing phase. These are cards that got tagged using `Git`.

### Card Flow

_WIP_ Draw a diagram here

## Board Swimlanes

It is a horizontal categorization of issues in the active Sprints of a Board. We can use it to help distinguish tasks of different categories, such as users, applications areas, etc.

We can split it via:

1. Stories
2. Hotfix
3. Bug
4. Expedite

### Card Organization

We can make use of Jira. In it you make use of `Component`.

Using Components we can organize the card by Specialties.

For example:

1. Operations
2. Projection
3. Test Automation

#### First, create a component

_PUT AN IMAGE HERE_

## Resources

1. [Scaled Agile Framework - Epic](https://www.scaledagileframework.com/epic/)
2. [Atlassian's Agile Tutorial - Epic](https://www.atlassian.com/agile/tutorials/epics)
3. [Atlassian's Project Management' Epics, Stories, and Themes](https://www.atlassian.com/agile/project-management/epics-stories-themes)
4. [Naming Task, Bug, and User Story Titles](https://stratejos.ai/blog/naming-task-bug-user-story-titles/)
5. [Atlassian's Agile Project Management - User Stories](https://www.atlassian.com/agile/project-management/user-stories)
