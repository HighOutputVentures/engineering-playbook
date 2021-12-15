# Reviewer's Checklist

* The correctness of the business logic embodied in the code.
* The correctness of any new or changed tests.
* The readability and maintenance of the overall design decisions are reflected in the code.
* The checklist of common errors that the team maintains.

### General Guidance

#### Understand the code you are reviewing

* Read every line changed.
* Read the code in some logical sequence to aid understanding.
* If you don't fully understand a change in a file because you don't have context, click to view the whole file and read through the surrounding code or check out the changes and view them in a text editor or IDE.
* Ask the author to clarify.

#### Be considerate

* Be positive -- encouraging appreciation for good practices.
* Use "we" instead of "you". Code reviews are not personal and language matters.
* Prefer asking questions above statements. There might be a good reason for the author to do something.
* If you make a direct comment, explain why the code needs to be changed, preferably with an example.
* If a few back-and-forth comments don't resolve a disagreement, have a quick talk with each other (call). Don't forget to update the PR with what you agreed on and why.

#### Make comments clear

* Explain why the code needs to change.
* Suggest changes to a PR by using the suggestion feature
* If one or two comments don't resolve a disagreement, create a group discussion or threads.

#### Decide on a common standard for each language

* Automate as much as possible (styling, etc.) to avoid the for `"Nit's"` and allow the reviewer to focus more on functional aspects of the PR.

### First Pass

#### Pull Request Overview

* Does the PR description make sense?
* Do all the changes logically fit in this PR, or are there unrelated changes?
* If necessary, are the changes made reflected in updates to the README or other docs? Especially if the changes affect how they build the user code.

#### User Facing Changes

* If the code involves a user-facing change, is there an image that explains the functionality? If not, it might be key to validate the PR to ensure the change does what is expected.
* Ensure UI changes look good without unexpected behavior.

#### Design

* Do the interactions of the various pieces of code in the PR make sense?
* Does the code recognize and incorporate architectures and coding patterns?

### Code Quality Pass

#### Complexity

* Are functions too complex?
* Is the single responsibility principle followed? Functions or classes should do one 'thing'.
* Should a function be broken into multiple functions?
* If a function/method has greater than 3 arguments, it is potentially overly complex.
* Does the code add functionality that isn't needed?
* Can the code be understood easily by code readers?

#### Naming/readability

* Did the developer pick good names for functions, variables, etc.?

#### Error Handling

* Are errors handled gracefully and explicitly when necessary?

#### Functionality

* possible cause of race conditions.
* could the code be optimized?
* does the functionality fit in the bigger picture? Can it have negative effects on the overall system?
* Security flaws
* Does the variable name reveal any customer-specific information?
* Are we logging the customer's sensitive information?

#### Style

* Are there extraneous comments? If the code isn't clear enough to explain itself, then the code should be made simpler. Comments may be there to explain why some code exists.
* Does the code adhere to the style guide/conventions that have been agreed upon? We use automated styling like, `Pretter`.

#### Tests

* Tests should always be committed in the same PR as the code itself (‘I’ll add tests next’ is not acceptable).
* Make sure tests are sensible and valid assumptions are made
* Make sure edge cases are handled as well.
* Tests can be a great source to understand the changes. It can be a strategy to look at tests first to help you understand the changes better.
