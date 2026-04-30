---
title: "Structuring the Data: Designing Tasks and Progress Tracking"
date: 2026-04-30
author: "Yan LIU"
summary: "Exploring how data structure decisions support core functionality while maintaining simplicity."
tags:
  - data-design
  - erd
  - design-decisions
---


As the core functionality of the application becomes more defined, it is necessary to consider how data should be structured to support these features. While the application aims to remain simple, its underlying data model still plays a critical role in determining both usability and implementation complexity.

The primary functional requirements identified earlier include creating daily tasks, marking them as complete, and tracking progress over time. To support these features, I considered two possible approaches to structuring task and progress data.

The first approach is to separate tasks and progress into different data entities. In this model, tasks would be stored independently, while progress records would track when tasks are completed. This structure allows for more detailed analytics, such as tracking completion history over multiple days or generating insights into user behaviour. However, this approach introduces additional complexity. It requires managing relationships between entities, increasing both implementation effort and cognitive overhead when reasoning about the system.

The second approach is to combine task and progress information into a single, simplified structure. In this model, each task includes its own completion status and date. For example, a task could include fields such as description, completion status, and associated date. This approach reduces the need for managing relationships between separate data entities and simplifies both storage and retrieval.

At this stage, I have chosen the second approach. Given that the application does not include user accounts or complex analytics, a simplified data model is sufficient to meet the core requirements. This decision aligns with the overall design goal of minimizing cognitive load, not only for users but also within the development process itself.

To illustrate this, the data structure can be conceptualized as a single “Task” entity:

Task ID
Description
Date
Completion Status

This structure allows the system to easily display daily tasks and track completion without requiring complex queries or data transformations. It also supports the use of local storage, which was chosen in the previous design decision.

However, this simplified approach has limitations. It may not support more advanced features, such as tracking long-term trends or generating detailed progress reports. If such features become necessary in future iterations, the data model may need to be refactored into a more modular structure.

In conclusion, this decision demonstrates that data design is not only a technical concern but also a reflection of functional priorities. By choosing a simpler data structure, the application remains aligned with its core goal of reducing complexity while still supporting essential user needs. Future development may revisit this decision as requirements evolve.
