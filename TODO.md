
# User Story Mapping
> It is a dead simple idea. Talk about the user's journey through your product by building a simple model that tells your user's story as you do.
>
>    Jeff Patton 

<details>
<summary><b>Summary</b></summary>

<b>User Story Mapping</b> helps Agile team define what to build and maintain visibility for how it all fits together. They enable user-centered conversations, collaboration, and feature prioritization to align and guide iterative product development.
</details>

___

## Current Challenges
1. We have a meeting called Backlog grooming and it takes time.

2. We just make story cards from breaking down epic cards without knowing why do we need it.

3. We are quite reactive to UI/UX design to know the user flow.

4. The team does not have a shared understanding of the product.

## Motivation on why we need to use this and why is this beneficial for us.
1. **It puts the individuals working on it first** over what processes we incorporate and tools we should use.

2. **It helps us distinguish minimum requirements** over long-winded documentation about functionalities and requirements.

3. **Shortens feedback loop** by reducing chains of information.

4. **Quicky adapts** due to fast feedback, competitive analysis and product maturity.

5. **Identifying loopholes** due to not seeing the full picture of how the product is used.

6. A practice for **categorization, prioritization and refinement**.

## Benefits
The following are some of the ways that story mapping helps team improve their processes for building products that the user love.

### **Focuses on user value**

We are envisioning the perspective of the user. This way we can focus what efforts for the user to the best outcomes. An outside-in approach.

### **Prioritizes the right work**

Building a holistic visualization of all the work necessary to deliver product experience can help teams decide what is most important.

### **Drives clear, well-sized requirements**

We struggle on writing strong user stories and requirements. We can make bigger stories and break those stories into a smaller ones. With the samller workable items we can illustrate how these items fit together.

### **Delivers new value early and often**

We can group smaller stories into iterations and get feedback early on. This way we can know the value and task we should prioritize to have an impactful product.

### **Exposes risks and dependencies**

Due to having a holistic view of the product we have crutch for visualization about the potential blocks, risks and dependencies that should be mitigateed in order to have deliver a product.

### **Builds team consensus**

For each story we made, we have a shared view of a customer/user and the work that is required or improve. This kind of practice or exercise lead to shared understanding on what to build, when and why.

___

## First things First.

### Define the Right Product Owner
Product Owner should know what he wants

They have these 3 basic traits:
- Knowledgeable
- Empowered
- Engaged

### Build an Empathetic Developer Team

So that they can build a right solution for their product. 

They can also pitch simple but effective idea during the mapping of user stories.


> **NOTE**: Having these an Empathetic Team and a Directly Responsible Invdividual-Type of PO is a strong combination to meet small deadlines.

### Forget the terminilogies used in JIRA

Forget about the `THEMES`, `EPIC`, `STORY CARDS`, and `FEATURES`.

Don't introduce these to the Product Owner. Just tell them that we are just trying to model the users' perspective.

___


## How does USER STORY MAPPING work?

### How does user story mapping work
1. **Find out the different personas/type of users**

   It is better to determine different types of users or personas early on

   If the product's main users are for the blind people then you should carefully for accessibility.

   Find out who are the different personas

   **Examples**

         1. Admin
         2. Member
         3. Recruiter
         4. Job Seeker

2. **Frame the problem**

   Build a _backbone_ or _core ideas_ that make the product. 
   
   This is usually discussed by the **Product Owner** and **Product Designer**. Feel free to invite other member.

   **Example**:

         1. Authenticate User
         2. Manage User
         3. Job Candidate

3. **Map user activities**

   Add steps to complete the step above. Make sure to have this format:

   `[As a Person]`, `[I want to]`, `[so that]`.

      **Example**:

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
            

4. **Map user stories**

   We can add more granularity for discrete interactions of a step. 

   This will become a sizable requirement.

   **Example**:
   
         1. Authenticate User

            1. As an Admin, I want to register an Admin Role, so that I can have admin access.

               1. As an Admin, I want to enter valid username, so that I can have a unique username.

               2. As an Admin, I want to enter a valid password, so that I can have a strong passsword strength.

5. **Flow and prioritize**

Make use of colors and divide by swimlanes to indicate the value of that said stories

6. **Identify gaps, dependencies, technical requirements, and alternatives**

Collaborate with other members to enrich and validate the story map

7. **Plan for the prioritize items**

Plan items that are the top priority for development

### What are some challenges of user story mapping
- No clear customer
- No clear problem
- Limited Utility
- Re-work and redundancy
- Usage of different tools
  
### Philosophy
- Iterative AND Incremental

### TIPS
- Refrain from using `Themes`, `Epic`, `Functions`, and `Features`.
- Identify the Opening Game (Add backbones)
- Identify the Mid Game (Add steps to complete the backbone)
- Identify the End Game (Research, game changer)

> NOTE: Story maps are for breaking down big stories as you tell them.


## WHO PARTICIPATES

Anyone can participate in mapping user stories.

1. **Product Owner** should know what the customer wants.

2. **Product Designer** should know what kind of solutions he want to raise.

3. **Project Manager** is the one who set milestones, strategic roadmaps.

It is encourage to include the members when mapping the story. This will reduce loop holes

### You can spearate it by tags:
- Products
- Features
- Enhancements
- Specfications
- Requirements

1. Think
2. Write down the idea, _after thinking it_
3. Explain your idea
4. Place your idea on a card (Miro)

```
What is it?
Why build it?
What will happen?
When you do?

Desired Outcomes?
```

- List the types of Customers and Users.
- Types of users to a sentence or two about each
- Types of activities people would use the product for


1. Think of the core ideas of the product (Done by Product Owner and Product Designer)
   ```md
   # BIG STORY
   - Signing up
   - Change my service
   - Viewing my band stats
   - Working with my show calendar
   - Working with my audience
   - Viewing Promotions Online
   - Publicize Promotions
   ```
2. Think of the tasks that could complete that idea (Done by Product Designers)
   1. Focus on the breadth of the tasks that should be completed instead of the details of a certain task
   ```md
   # Viewing Promotions Online
   ```

## WHEN
1. Working on an MVP?
It is a great way to identify minimum requirements and functionality you need to test your concept.

2. Trying to Figure out how to improve on version 1.0?
A story map can visually display all of the potential enhancements you could add and help your team have quality conversations about what will most impact your users.

3. Managing your backlog a growing session?
Story mapping helps you tame the backlog by giving each item some context and forcing prioritization and grouping with a big-picture view; plus, it can highlight gaps you might have never noticed otherwise.

4. Branching out with a new product extension?
A story map will illustrate what you already have and the missing pieces you’ll need to make the new functionality work just as well as your current offering.


**FIRST STEP**
Regardless of whether your product is still theoretical or has been kicking around for decades, story mapping starts with personas -- you must know who will be using your product and what they're trying to accomplish.


## STORY MAPPING MYTHS
1. It has an end goal.
2. It eliminates loopholes.
3. It enables seamless collaboration.

### It has an end goal
Mapping stories are continuous. It will never be "done".

As we complete the steps, new ones get prioritized and additional steps are getting added.

Meanwhile, user feedback and competitve analysis uncover new requirements.

So whether you leave your story map up/out and update it or rebuild it from scratch periodically, the "backbone" and "key steps" remain part of the process.

### It eliminates loopholes

### It enables seamless collaboration


## User Story Mapping as Backlog Refinement
1. Arrange the top items on your product backlog to represent the prioritized items
2. Don't include any task lower than second-level priority on the backlog
3. Create a separate list of those lower-priority ideas and requests.
4. Re-evaluate the level one and two items on your backlog regularly


## Challenges if we incoroporate this in our workflow
1. Jira have flat backlogs
2. We might use 2 different tools
3. Jira does not have color indicator

## Resources
1. https://www.nngroup.com/articles/user-story-mapping/
2. https://www.productplan.com/glossary/story-mapping/
3. https://www.aha.io/roadmapping/guide/release-management/what-is-user-story-mapping
4. https://www.jpattonassociates.com/story-mapping/
5. https://medium.com/@lynxluna/what-make-agile-team-not-agile-52906f8c7408
6. https://storiesonboard.com/
8. https://medium.com/usabilitygeek/how-to-cope-with-multiple-user-flows-in-a-user-story-mapping-4a69c61d39e0
9. https://www.notion.so/highoutput/Authefy-82099844553b4168bbe8928701c53ef9
10. https://www.visual-paradigm.com/guide/agile-software-development/what-is-user-story-mapping/
11. https://www.productplan.com/learn/prioritize-product-backlog/
12. https://go.productplan.com/product-strategy-playbook/
