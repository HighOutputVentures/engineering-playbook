# Backlog Management

## Sections

1. Backlog Refinement
   1. User Story Mapping

## Backlog Refinement

Although there are several ways to groom and refine the backlogs, we must still pick a way where we can refine more and collaborate at the same time.

### 🥅 Goals

The team review the items on the backlog to ensure that the backlog that they are prioritized by the user's demands. This activity occurs on a regular basis and maybe an officially scheduled meeting or an ongoing activity.

### User Story Mapping

**Summary**

**User Story Mapping** helps the Agile team define what to build and maintain visibility for how it all fits together. They enable user-centered conversations, collaboration, and feature prioritization to align and guide iterative product development.

> It is a dead simple idea. Talk about the user's journey through your product by building a simple model that tells your user's story as you do.
>
> Jeff Patton

***

### Current Challenges

1. We just make story cards just for the sake of breaking down _Epic Cards_ without knowing the purpose of it.
2. We are quite reactive to UI/UX design to know the user flow.
3. The team does not have a shared understanding of the product.

### Motivation on why we need to use this and why is this beneficial for us.

1. **It puts the individuals working on it first** over what processes we incorporate and tools we should use.
2. **It helps us distinguish minimum requirements** over long-winded documentation about functionalities and requirements.
3. **Shortens feedback loop** by reducing chains of information.
4. **Quickly adapts** due to fast feedback, competitive analysis, and product maturity.
5. **Identifying loopholes** due to not seeing the full picture of how the product is used.
6. A practice for **categorization, prioritization, and refinement**.

### First Things First.

#### Define the Right Product Owner

Product Owner should know what he wants

They have these 3 basic traits:

* **Knowledgeable**
* **Empowered**
* **Engaged**

#### Build an Empathetic Developer Team

So that they can build the right solution for their product.

They can also pitch simple but effective ideas during the mapping of user stories.

> **NOTE**: Having these an Empathetic Team and a Directly Responsible Invdividual-Type of PO is a strong combination to meet small deadlines.

#### Forget the terminologies used in JIRA

Forget about the `THEMES`, `EPIC`, `STORY CARDS`, and `FEATURES`.

Don't introduce these to the Product Owner. Just tell them that we are just trying to model the users' perspective.

***

### How does USER STORY MAPPING work?

1.  **Find out the different personas/type of users**

    It is better to determine different types of users or personas early on

    If the product's main users are for the blind people then you should carefully for accessibility.

    > This is usually discussed by the **Product Owner** and **Product Designer**. Feel free to invite other members.

    Find out who are the different personas

    **Examples**

    ```
      1. Admin
      2. System
      3. Member
      4. Recruiter
      5. Job Seeker
    ```
2.  **Frame the problem**

    Build a _backbone_ or _core ideas_ that make the product.

    > **💡 Advisory Note**
    >
    > This is usually discussed by the **Product Owner** and **Product Designer**. Feel free to invite other members.

    **Example**:

    ```
      1. Authenticate User
      2. Manage User
      3. Job Candidate
    ```
3.  **Map user activities**

    Add steps to complete the step above. Make sure to have this format:

    > **💡 Advisory Note**
    >
    > This can be done by the **Product Designer** and can be collaborated with other other members.

    ```
    [As a Person], [I want to], [so that].
    ```

    **Example**:

    ```
         1. Authenticate User
            1. As an Admin, I want to register an Admin Role, so that I can have admin access.

            2. As an Admin, I want to have a traditional login, so that I can have access.

            3. As a Member, I want to receive an invitation link, so that I can register with my email.

            4. As a Member, I want to have a passwordless login, so that I only have less concern.

         2. Manage User
            1. As an Admin, I can invite a user, so that I can have a list of users under a project.

            2. As an Admin, I can see the list of users, so that I can manage them well.

            3. As an Admin, I can see more details of a user, so that I can revoke access or edit the profile of selected user.

         3. Recruit Candidate
            1. As a Recruiter, I can search for candidates, so that I can have a pool of candidate to a vacant job.

            2. As a Recruiter, I can contact a candidate, so that I can share details about the company and the vacant job.
         
    ```
4.  **Map user stories**

    We can add more granularity for discrete interactions of a step.

    This will become a sizable requirement.

    > It is recommended that all members should participate in this.
    >
    > This will allow us to highly find potential discrepancies.

    **Example**:

    ```
      1. Authenticate User

         1. As an Admin, I want to register an Admin Role, so that I can have admin access.

               1. As an Admin, I want to enter valid username, so that I can have a unique username.

               2. As an Admin, I want to enter a valid password, so that I can have a strong passsword strength.
    ```
5.  **Flow and prioritize**

    Make use of colors and divide by swimlanes to indicate the value of that said stories
6.  **Identify gaps, dependencies, technical requirements, and alternatives**

    Collaborate with other members to enrich and validate the story map
7.  **Plan for the prioritized items**

    Plan items that are the top priority for development

### What are some challenges of user story mapping?

1.  Limited Utility

    There are some tools that can use for a decent mapping of user stories.

    For example, [Avion](https://www.avion.io) and [Feature Map](https://www.featuremap.co/en).
2.  Rework and redundancy

    Making adjustments and refining the user story mapping is a tedious and redundant work
3.  Usage of different tools

    If we try to integrate using some add-on tools for Jira we can eliminate this.

    The following add-ons would be:

    1. [Agile User Story Map PRO for Jira](https://marketplace.atlassian.com/apps/1211098/agile-user-story-map-pro-for-jira?hosting=cloud\&tab=overview)
    2. [Easy Agile](https://www.easyagile.com/blog/the-ultimate-guide-to-user-story-maps/)

### TIPS

* Refrain from using `Themes`, `Epic`, `Functions`, and `Features`.
* Identify the Personas.
* Identify the _Opening Game_ (Add backbones)
* Identify the _Mid Game_ (Add steps to complete the backbone)
* Identify the _End Game_ (Research, game changer)

> NOTE: Story maps are for breaking down big stories as you tell them.

### WHO PARTICIPATES

Anyone can participate in mapping user stories.

1. **Product Owners** should know what the customer wants.
2. **Product Designers** should know what kind of solutions they want to raise.
3. **Project Manager** is the one who sets milestones, strategic roadmaps.
4. **QAs** are the one finding faults by testing the product.
5. **Developer** are the one who completes the user stories.

It is encourage to include ALL the members when mapping the user stories. This will reduce loopholes.

***

### WHEN CAN WE USE IT?

1.  **Working on an MVP**?

    It is a great way to identify the minimum requirements and functionality you need to test your concept.
2.  **Trying to Figure out how to improve on version 1.0**?

    A story map can visually display all of the potential enhancements you could add and help your team have quality conversations about what will most impact your users.
3.  **Managing your backlog a growing session**?

    Story mapping helps you tame the backlog by giving each item some context and forcing prioritization and grouping with a big-picture view; plus, it can highlight gaps you might have never noticed otherwise.
4.  **Branching out with a new product extension**?

    A story map will illustrate what you already have and the missing pieces you’ll need to make the new functionality work just as well as your current offering.

> **💡 A better first step**
>
> Regardless of whether your product is still theoretical or has been kicking around for decades, **story mapping starts with personas -- you must know who will be using your product and what they're trying to accomplish**.

### USER STORY MAPPING MYTHS

1.  This work is only for the Product team or UI/UX team.

    **No, it's a collaborative work where the core features are initially set up by the product owners and product designers**. Verification and elimination of redundancies are done by the whole team.
2.  It can ONLY be done at the start of the project.

    User story mapping is reliable even for the existing projects or even for the projects that only have internal users.
3.  It is a way of gathering user requirements.

    User story mapping is NOT the way to gather user requirements. It is a way to gather users' demands. By doing this, we can distinguish what features have the biggest impact.

    A supercharged story mapping is used together with Agile Framework **Kanban + Pull System Task Assignment**.

    **Kanban** - by limiting cards based on the user's demands that comes from the User Story Mapping and by making use of board column limits.

    **Pull System** - to set our own pace, based on the refined cards, this will avoid waste so that you can allocate manpower and resources well.
4.  It has an end goal.

    Mapping stories are continuous. It will never be "done".

    As we complete the steps, new ones get prioritized and additional steps are getting added.

    Meanwhile, user feedback and competitive analysis uncover new requirements.

    So whether you leave your story map up/out and update it or rebuild it from scratch periodically, the "backbone" and "key steps" remain part of the process.
5.  It eliminates loopholes.

    It does not eliminate discrepancies or loopholes but **greatly reduces them**.
6.  It enables seamless collaboration.

    It does not create a seamless collaboration but **shortens the feedback loop**.

    It is easy to be distracted by a minute detail and it is advised to have an initiator or some kind of facilitator in this session.

### User story mapping vs Event Storming

Event Storming is more high-level than User Story Mapping.

Event Storming should be done early so we can write down business events, commands that trigger those events, and reactions.

User Story Mapping, on the other hand, the main focus is to refine the backlog to deliver an MVP or working product based on the user's journey.

### User story mapping vs journey mapping

Journey mapping is for UX designers where they value the experience of the users more rather than the holistic view of the product.

It is more focused on the single persona or customer.

Unlike User Story Mapping, it focuses more on the whole vision of the product taking by using user experience as a crutch.

### Challenges if we incorporate this in our workflow

1. Jira has flat backlogs
2. Lack of utility product for User story mapping
3. We might use 2 different tools
4. Jira does not have a color indicator

## Minimalism

* Split your work item into small chunks that are contributed in incremental commits.
* Contribute your chunks frequently. Follow an iterative approach by regularly providing updates and changes to the team. This allows for instant feedback and early issue discovery and ensures you are developing in the right direction, both technically and functionally.
* Do NOT work independently on your task without providing any updates to your team.

### Resources

1. https://www.nngroup.com/articles/user-story-mapping/
2. https://www.productplan.com/glossary/story-mapping/
3. https://www.aha.io/roadmapping/guide/release-management/what-is-user-story-mapping
4. https://www.jpattonassociates.com/story-mapping/
5. https://medium.com/@lynxluna/what-make-agile-team-not-agile-52906f8c7408
6. https://storiesonboard.com/
7. https://medium.com/usabilitygeek/how-to-cope-with-multiple-user-flows-in-a-user-story-mapping-4a69c61d39e0
8. https://www.notion.so/highoutput/Authefy-82099844553b4168bbe8928701c53ef9
9. https://www.visual-paradigm.com/guide/agile-software-development/what-is-user-story-mapping/
10. https://www.productplan.com/learn/prioritize-product-backlog/
11. https://go.productplan.com/product-strategy-playbook/
12. https://www.easyagile.com/blog/the-ultimate-guide-to-user-story-maps/
13. https://www.jpattonassociates.com/qa\_branches\_in\_maps/
14. https://www.justinmind.com/blog/user-story-mapping/
15. http://minifesto.org/
