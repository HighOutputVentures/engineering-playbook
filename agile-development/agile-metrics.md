# Agile Metrics

### Main Metrics

#### Cycle Time&#x20;

Is the time your team spends actively on the client's request

![ ](<../.gitbook/assets/Screen Shot 2022-01-03 at 10.39.06 AM.png>)

In Kanban, this is where we calculate the card from In **Progress** to **Done.**  It is important to note that cycle time can be calculated in different issue types.

\
**`Cycle Time = Start Date Time - End Date Time`**

We also need to measure the **Average Cycle Time** so that we could answer in a situation where the business owners asked how long the feature will take.

**Average Work In Progress = No. of  story cards started but not finished**

**Example:**

* Monday - 3
* Tuesday - 4
* Wednesday - 3
* Thursday - 2
* Friday - 2

**`Average Work In Progress = (1 + 1 + 2 + 2 + 2) / 5`**

**`Average Work In Progress = 2.8 (3 WIP cards per day)`**

****

**`Average Throughput = No. of done story cards per unit of time`**

**Example:**

* Monday - 1
* Tuesday - 1
* Wednesday - 2
* Thursday - 3
* Friday - 2

**`Average Throughput = (1 + 1 + 2 + 3 + 2) / 5`**

**`Average Throughput = 1.8 (2 cards per day)`**



**`Average Cycle Time = Average Work In Progress / Average Throughput`**

**`Average Cycle Time = 3 / 2`**

**`Average Cycle Time = 1.5 ( 2 days to finish a story card)`**

#### ``

#### Change of Failure Rate

The percentage rate of code changes that require hotfixes after production.

#### **Defects found after release to customers**

Bugs found after the release to the customers

#### **Mean Time to Detect**

Mean amount of time it takes for the team to discover or detect an incident.

#### **Defects Found During Development**

Bugs found during development

### **Other Metrics**

1. **Percentage of Uptime -** gives you an idea of the percentage of the total time that the processes are actually active
2. **Lead time for changes** - from the request to the client getting the value
3. **Setup Time** - is the amount of time needed to prepare for a given step
4. **Takt time** - is the maximum amount of time the team needs to comply to meet the client demands
5. **Deployment Frequency** - frequency of the new code is deployed into production
6. **Mean Time to Failures** - the average time between repairable failures.
7. **Mean Time to Recover** - measure how long it takes to recover from a partial service interruption or total failure
8. **Mean Time to Repair** - is the average time it takes to fix an application
9. **Mean Time to Resolve** - is the average time it takes to completely fix an application that makes sure it does not repeat again.
10. **Mean Time to Acknowledge** - is the average from detection to the start of working it.
