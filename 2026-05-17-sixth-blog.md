---
title: "Integrating Community Features within a Low Cognitive Load Task System"
date: 2026-05-17
author: "Yan LIU"
summary: "Defining how a required community feature is implemented within an ADHD-focused productivity system while maintaining low cognitive load, usability, and accessibility constraints."
tags:
  - functional-requirements
  - accessibility
  - design-decisions
---

Defining functional requirements for community interaction

The application is designed as a task management system for students with attention difficulties such as ADHD. The core functionality includes creating tasks, tracking completion, and monitoring progress over time. In addition to these core features, the BlaBla design brief requires the inclusion of a community feature to support user interaction and shared experiences.

However, introducing community functionality creates a design challenge: social interaction can improve motivation but also increase cognitive load. As a result, the implementation must balance interaction requirements with accessibility constraints.

Simplified community system design

The community system is implemented using a lightweight CommunityPost structure that stores short text messages, optional usernames, and timestamps. The system supports encouragement messages, study tips, and optional mood check-ins.

To satisfy the requirement while maintaining usability, more complex social features have been deliberately excluded, including:

real-time chat systems
comment threads
likes or ranking mechanisms
algorithmic content feeds

These features were removed because they would increase cognitive load, introduce distraction, and conflict with the ADHD-focused design goal of maintaining a calm and predictable interface.

Instead, the community system is designed as a simplified interaction layer that still fulfils the required social function without dominating the user experience.

System architecture and implementation

The application architecture is structured into three functional layers:

Task system: core productivity functionality (create, complete, delete tasks)
Timer system: focus support and time management
Community system: lightweight interaction and motivation layer

All data is stored using localStorage, avoiding backend complexity and ensuring fast, responsive interactions. This supports the design goal of reducing both technical and cognitive complexity.

Figure 1: System architecture and functional hierarchy

<img width="481" height="441" alt="b6" src="https://github.com/user-attachments/assets/6af2c985-974c-415a-ba50-e02caac724c1" />

Figure 1 caption:

The diagram illustrates the system architecture and functional hierarchy. It shows how the required community feature is implemented as a constrained layer alongside the core task and timer systems. This ensures that social interaction supports motivation without interfering with primary productivity workflows, maintaining low cognitive load for ADHD users.

Accessibility considerations

Accessibility is treated as a functional requirement of the system. In addition to standard visual accessibility requirements such as contrast and readability, the design also addresses cognitive accessibility by reducing interface complexity and ensuring consistent interaction patterns.

Optional accessibility features include:

speech support
large text mode
colour-blind mode

These features are implemented without interfering with the default simplified experience.

Evaluation will include WCAG-based accessibility testing Web Content Accessibility Guidelines (WCAG), screen reader testing, and keyboard-only navigation testing.

Evaluation approach

The system will be evaluated using both automated and manual methods.

Automated evaluation includes:

accessibility audits (WCAG compliance)
Lighthouse performance testing
code structure validation

Manual evaluation focuses on user task performance:

task creation, completion, and deletion
timer usage and focus tracking
interaction with community posts
keyboard-only navigation testing

Success is defined by whether users can complete core workflows with minimal cognitive effort rather than feature richness.

Ethical and data considerations

The application stores all data locally using localStorage and does not collect external personal data. This reduces privacy risks and aligns with data minimisation principles under the Australian Privacy Act 1988.

Community posts are not ranked, profiled, or algorithmically manipulated, reducing risks of engagement bias and behavioural tracking.

Summary

The system is designed to meet both functional and accessibility requirements by integrating a required community feature in a simplified and constrained form. This ensures that the application supports productivity, focus, and social interaction simultaneously, without compromising usability for students with attention difficulties.
