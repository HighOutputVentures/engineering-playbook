# Writing an Acceptance Criteria

## Standard

#### One Scenario should only have one result

```gherkin
# Bad example

Scenario: Simple product search
    Given the shoe store, the home page is displayed
    When the search phrase "red pumps" is entered
    Then results for "red pumps" are shown
    When the user searches for images from the results page
    Then image results for "red pumps" are shown
```

It has two results since it has two `When-Then`.

Separating `When-Then` into two scenarios would create one result for each scenario.

```gherkin
# Good example

Scenario: Simple Web search
    Given the shoe store, the home page is displayed
    When the search phrase "red pumps" is entered
    Then results for "red pumps" are shown

Scenario: Simple Web image search
    Given shoe store search results for "red pumps" are displayed
    When the user searches for images from the results page
    Then image results for "red pumps" are shown
```

This is easy to trace because **each failure points to a unique problem**.

It is concise and more focus on a particular scenario.

> **💡 Advisory Note:**
>
> #### The Cardinal Rule of BDD: One Scenario, One Behavior!
>
> `1 behavior -> 1 example -> 1 scenario -> 1 test -> 1 result`

#### Deliver it in declarative form, enough to have descriptive steps

```gherkin
# Bad example

Scenario: Shoes
  Given I want shoes
  When I buy shoes
  Then I get them
```

This is a declarative form, BUT **too vague and ambiguous**.

```gherkin
# Bad example

Scenario: Purchase shoes through the app
  Given my username is "jessica8494"
  And my password is "PleaseDontPutSecretsInGherkin"
  When I navigate the browser to "www.shoestore.com"
  And I enter my username into the "Username" field
  And I enter my password into the "Password" field
  And I click the login button
  And I wait "10" seconds
  Then the Shoe Store home page is displayed
  And the title banner contains the text "Shoe Store"
  And the shopping cart is empty
  When I click the search bar
  And I type "red pumps" into the search bar
  And I click the search button
  And I wait "30" seconds
  Then the search results page is displayed
  And the search results page shows "10" results per page
  And ...
```

Now take this another example, a complete opposite of the previous one. This is written in an imperative form and **it is too descriptive**.

```gherkin
# Good example

Scenario: Add shoes to the shopping cart
  Given the shoe store, the home page is displayed
  When the shopper searches for "red pumps"
  And the shopper adds the first result to the cart
  Then the cart has one pair of "red pumps"
```

This example, have the right balance **to be declarative and at the same time has clear steps**.

#### Make use of the data table to display unique examples

```gherkin
# Good example

Scenario Outline: Invalid Password
  Given the password contain <invalid-format>
  When the user navigates to another field
  Then it would notify an error

   | invalid-format |
   | -------------- |
   | test           |
   | 123            |
   | teeest123      |
   | qwetest123     |
```

#### Make use of the third person and be consistent throughout the scenario

```gherkin
# Good example

Scenario: Guests only see the promos
  Given the guest is unregistered.   
  When the guests apply to a promo
  Then he sees an error pop up message
```

This example, have a clear persona.

#### Remove ambiguity

```gherkin
# Bad example

Scenario: ...
    Given ...
    When ...
    Then image and video links for "sneakers"
```

It has an ambiguous result, clarify it like this:

```gherkin
# Good example

Scenario: ...
    Given ...
    When ...
    Then the results page shows image and video links for "sneakers"
```

It explicitly tells you what exactly happens. The example above makes the readers reduce the potential assumptions.

#### Make it consistent

Take note of these steps and it's intention.

* `Given` steps **should use past or present-perfect tense** because they represent an initial state that must already be established.
* `When` steps **should use the present tense** because they represent actions actively performed as part of the behavior.
* `Then` steps **should use the present or future tense** because they represent what should happen after the behavior actions.

### Resources

1. [Better Behavior Driven Development -- 4 Rules Writing Good Gherkin](https://techbeacon.com/app-dev-testing/better-behavior-driven-development-4-rules-writing-good-gherkin)
2. [Are Gherkin Scenario with Multiple When-Then Pairs Okay](https://automationpanda.com/2018/02/03/are-gherkin-scenarios-with-multiple-when-then-pairs-okay/)
3. [Should gherkin steps use first-person or third-person?](https://automationpanda.com/2017/01/18/should-gherkin-steps-use-first-person-or-third-person/)
4. [BDD -- Collaboration without automation](https://automationpanda.com/2017/07/26/bdd%E2%80%91%E2%80%91-collaboration-without-automation/)
5. [BDD -- Automation without Collaboration](https://automationpanda.com/2017/07/26/bdd-automation-without-collaboration/)
6. [BDD Example Mapping](https://automationpanda.com/2018/02/27/bdd-example-mapping/)
7. [What is a good feature or user story template](https://www.aha.io/roadmapping/guide/requirements-management/what-is-a-good-feature-or-user-story-template)
