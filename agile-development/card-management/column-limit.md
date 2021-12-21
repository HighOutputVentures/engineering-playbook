# Column Limit

Add limit to the columns to control and encourage prioritization when the limit is reached.

> **⚠️ TAKE NOTE:**&#x20;
>
> The default numbers presented below are considered as a baseline to start off a project or adding WIP limit to an existing project.\
> \
> It can be adjusted based on your team size and velocity.

### Determining the Column Limit

Please determine the Total Value Adding (VA): 20 days

Please determine the Total Non-Value Adding (NVA): 10 days

Please determine how many team members: 4

#### Get the Efficiency

```
Efficiency = VA / (VA + NVA)
```

Get the `Total WIP Limit`

```
Total WIP Limit = Number of Team Members / Efficiency
```

Get the % of Total VA

```
% of Total VA = (VA / Total VA) * 100
```

Get the WIP Limit for each column

```
WIP Limit of a column = % Total VA * Total WIP Limit
```

| Columns        | Value Adding | % of Total Value Adding | WIP Limit |
| -------------- | ------------ | ----------------------- | --------- |
| To Do          | 3            | 15%                     | 3         |
| In Progress    | 10           | 50%                     | 10        |
| Ready For QA   | 1            | 5%                      | 1         |
| QA In Progress | 3            | 15%                     | 3         |
| QA Failed      | 2            | 10%                     | 2         |
| Done           | 1            | 5%                      | -         |

### Resources

1. [Kanbanize - WIP Limits](https://kanbanzone.com/resources/kanban/wip-limits/)
