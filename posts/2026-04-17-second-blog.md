---

Title: Defining Core Functional Requirements: What is Essential and What is Optional?

Date: 2026-04-17

Author: Yan LIU

Summary: Identifying essential features and managing scope through prioritization and trade-offs.

Tags:

- functional-requirements

- scope
- design-decisions

---

Following the previous article's initial exploration of user needs, the next step is to define the application's functional requirements. A key challenge in this process is distinguishing between core and optional functions. Failure to do so risks exceeding the project's feasible scope and reducing design clarity.

Based on the needs of students with attention deficit disorder, we have summarized several core functional requirements. First, the application must allow users to create and manage a small number of daily tasks. This is crucial because task organization is a fundamental problem faced by the target users. Second, the system should provide a simple way to mark tasks as completed. This helps users gain a sense of accomplishment and progress, thus maintaining motivation. Third, the application should include basic progress tracking functions, such as daily completion records or summaries, to encourage long-term user engagement.


In contrast, some of the initially considered features may not be essential. For example, a learning resource sharing system where users can upload and browse learning materials. While this could add value, it would significantly increase the application's complexity. It would require additional data structures, user management, and interface design, which might not be directly related to the core goals of improving focus and task completion rates.

Another optional feature is social interaction, such as commenting or liking shared content. While these features are common in many applications, they could be unnecessarily distracting for the target users. From a design perspective, this could conflict with the goal of reducing cognitive load.

Given these considerations, I decided to prioritize a set of the most basic core features in the initial version of the application. Optional features, such as resource sharing, will be considered as potential future expansions, rather than current necessities. This decision reflects a trade-off between functionality and usability, and between ambition and feasibility.

It's important to note that this is not simply narrowing down the scope, but rather a thoughtful design choice based on user needs. By focusing on core functionality, the application can offer a clearer, more human-centered user experience. Furthermore, this approach allows us to more carefully evaluate the performance of core features before introducing further complexity.

In future development phases, if evidence suggests that these optional features can improve the user experience without compromising design simplicity, I may reconsider adding them. Currently, maintaining a clear and well-defined scope is crucial for the project's success.
