---
title: “Balancing Simplicity and Functionality: Do We Need User Accounts?”
date: 2026-04-25
author: “Yan LIU”
summary: “Evaluating whether user authentication is necessary for a low-cognitive-load study tracking application.”
tags:
  - design-decisions
  - architecture
  - authentication
  - trade-offs
---

As the application's functional requirements become clearer, an important design decision emerges: whether the system should include user accounts and authentication. While this feature is common in many web applications, its necessity in this specific context is not immediately obvious.

On the one hand, implementing a user account system provides several clear advantages. It allows users to store their task data persistently across devices and sessions. This would support long-term progress tracking, which aligns with the previously identified requirement of maintaining user motivation over time. Additionally, authentication enables more advanced features in the future, such as personalized insights or cloud-based backups.

However, introducing user accounts also brings significant trade-offs. From a user experience perspective, requiring registration and login adds friction to the interaction flow. For students with attention difficulties, even small barriers can reduce engagement or discourage consistent use. This directly conflicts with the design goal of minimizing cognitive load and simplifying user interaction.

From a technical perspective, authentication substantially increases system complexity. It requires secure handling of user credentials, session management, and potentially backend infrastructure such as databases and APIs. Given the limited scope of this prototype and current development constraints, this added the immediate benefits may not justify the complexity.

An alternative approach is to avoid user accounts entirely in the initial version of the application. Instead, task data could be stored locally within the browser (e.g., using local storage). This would allow users to quickly access and use the application without any setup process. While this limits cross-device access and long-term data persistence, it significantly simplifies both the user experience and the technical implementation.

At this stage, I have chosen to adopt the second approach and exclude user authentication from the initial design. This decision prioritizes accessibility and ease of use over extended functionality. It reflects a clear alignment between the application's core requirement—supporting focus and reducing cognitive load—and the technical design choices.

That said, this decision is not without limitations. The lack of persistent, account-based data may reduce the application's usefulness for long-term tracking. In future iterations, it may be necessary to revisit this decision if user needs evolve or if additional features require more robust data management.

In conclusion, this design decision illustrates the importance of evaluating not only what a system can do, but what it should do within a given context. By deliberately limiting functionality, the application can better serve its intended users and remain aligned with its core design principles.
