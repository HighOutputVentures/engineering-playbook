# User story

A user story is a behavior or feature that a solution needs to implement in order to fulfill the needs, from the user's perspective.

### Why should we create it?

1. It **keeps focusing on the user**.
2. It **enables collaboration**.
3. It **drives creative solutions**.
4. It **creates momentum**.

### Naming title guidelines

Make the title _declarative_.

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

As a Creator, I want to announce my newly created profile to Bitclout, so that they are aware I signed up on Jamclout.



Add more details to eliminate assumptions.

#### Acceptance Criteria

Make use of `Gherkin`'s syntax by using `GIVEN`, `WHEN`, `THEN` and many more.

1. It should be written in 3rd Person
2. Each step should be declarative
3. Each should define a scenario

**Example(s)** Scenario: PENDING requests cannot be approved immediately

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
