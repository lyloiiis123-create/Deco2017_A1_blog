---
title: "Revisiting Earlier Assumptions: Balancing Future Expansion and Design Simplicity"
date: 2026-05-14
author: "Yan LIU"
summary: "Reflecting on earlier design decisions and evaluating how future feature expansion may affect usability, cognitive load, and technical complexity."
tags:
  - design-reflection
  - trade-offs
  - scalability
---

Revisiting Earlier Assumptions: Balancing Future Expansion and Design Simplicity

As development planning progresses, it becomes increasingly important to revisit earlier assumptions and evaluate whether the current design direction still aligns with the application's core goals. Although previous decisions focused heavily on limiting complexity and reducing cognitive load, further reflection reveals that maintaining simplicity over time may become more difficult as additional features are considered.

One of the major challenges in software design is that applications often grow beyond their original scope. Features that initially appear useful can gradually increase interface complexity, technical maintenance requirements, and user distraction. This issue is particularly important for this project because the target users—students with attention difficulties—may be negatively affected by overly complicated interfaces or inconsistent interaction patterns.

Earlier blog posts identified several features as optional, including social interaction systems, resource sharing, and account-based synchronization. At the time, excluding these features appeared to be the most appropriate decision due to both technical limitations and usability concerns. However, revisiting these assumptions highlights that some optional features may eventually provide meaningful value if implemented carefully.

For example, progress visualisation was initially considered potentially distracting because excessive charts or statistics could increase cognitive load. However, after further consideration, a very minimal form of progress feedback may actually improve user motivation without introducing significant complexity. A simple visual indicator, such as a daily completion bar or streak counter, could help users recognise small achievements and encourage consistent study habits.

This introduces an important design trade-off. Providing feedback can improve motivation and long-term engagement, but excessive feedback systems may unintentionally create pressure or anxiety. Many productivity applications rely heavily on gamification techniques such as achievement systems, notifications, and competitive tracking. While these systems may increase engagement for some users, they may also become overwhelming or distracting for students who already struggle with attention regulation.

As a result, any future expansion of the application should follow the same principle established in earlier design decisions: additional functionality should only be introduced if it directly supports the user's core needs without significantly increasing cognitive complexity. This means that future features should remain lightweight, predictable, and optional wherever possible.

This reflection also affects technical planning. Although the current simplified data structure and local storage approach are sufficient for the prototype, future expansion may eventually require a more scalable architecture. For example, if long-term progress tracking or cross-device synchronization becomes necessary, the application may need a database-backed system and user authentication. However, introducing these systems too early could increase implementation complexity before their value is clearly justified.

At this stage, the project continues to prioritise clarity and feasibility over feature expansion. Revisiting earlier assumptions has reinforced that successful design is not about continuously adding functionality, but about carefully evaluating whether each addition genuinely improves the user experience.

Ultimately, this process demonstrates that design decisions should remain flexible and open to reassessment throughout development. Rather than treating early decisions as fixed, it is important to continually reflect on how well the application aligns with its original purpose: supporting students with attention difficulties through a simple, focused, and accessible learning environment.

<img width="261" height="211" alt="Untitled Diagram drawio" src="https://github.com/user-attachments/assets/a71a1932-7f99-4fe7-9ae6-56bd5e4a5fec" />

