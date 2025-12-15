---
layout: essay
type: essay
title: "Thank you - ICS 314"
date: 2025-12-14
published: true
labels:
  - Software Engineering
  - Reflection
  - Coding Standards
  - Ethics
  - Functional programming
---

<img width="300px" class="rounded float-start pe-4" src="../img/software.jpeg">

# Introduction

What a ride. If you had asked me four months ago whether I wanted to be a software engineer, I would have said, "maybe — let's see how that goes." As I near the end of ICS 314, I realize I have learned a great deal about modern web application development. More importantly, I discovered that the foundational concepts of software engineering are the deeper value of this class. In addition to building projects with React, Next.js, TypeScript, and PostgreSQL, I deeply connected with broader ideas that apply to software systems of any scale. Three topics in particular — functional programming, coding standards, and design patterns — were the most important concepts I took away from the course.

# Functional Programming

Functional programming emphasizes writing software by composing pure functions. During the first weeks of JavaScript and TypeScript introduction, I learned to adopt a functional mindset. Functions like map, filter, and reduce encouraged me to add new techniques to my coding toolbox. Through continuous concept introductions and WODs (practice!), I learned to write cleaner, more predictable, and more consistent functional code.

One clear example from my group project was transforming data fetched from the database. When retrieving running routes, user stats, or profile information, we needed to convert raw database results into useful shapes. Rather than mutating objects and variables directly, we used functions like `.map()` and `.filter()` to transform data immutably and clearly.

# Coding Standards 

Coding standards are universal guidelines for how code should be written, organized, and formatted. Standards ensure that in a group project, code remains readable, maintainable, and consistent despite differing skill sets and habits. As our group progressed, I came to appreciate ESLint and its rigorous rules for how we write code. When multiple contributors work on different issues that can conflict, it is important that anyone can open a file and understand it quickly. Because my group consistently practiced proper coding standards and procedures, we avoided those problems.

Before ICS 314, I thought linting was tedious because I preferred my own indentation and formatting. Early in the semester, during a practice WOD, a friend had trouble tracing my code because it was organized only for my preference. That experience made me appreciate linting tools and how they promote collaboration and reduce confusion.

Linting helps prevent small mistakes from growing into deeply rooted problems that are hard to fix and hard to read. As I move forward in software engineering and other areas of computer science, I will ensure coding standards are implemented in my projects and acknowledged by teammates.

# Design Patterns

Similar to the base case in a dynamic programming problem or the structural template of a house, a design pattern is a reusable, standardized solution to a common problem.  A design pattern offers a conceptual blueprint that may be modified according to the project's requirements, as opposed to a rigid piece of code. Certain fundamental structures are necessary for usability, clarity, and consistency in software engineering, architecture, and even physical design.  For instance, almost all contemporary homes have a kitchen, a bathroom, a bedroom, water, and electricity.  Without these common design components, a home would be confusing or dysfunctional.

In software, design patterns offer the same consistency.  They enhance maintainability, establish expectations, and speed up developers' comprehension of new projects.  Additionally, they stop mistakes from happening again; maintaining a solid pattern builds long-term proficiency and results in systems that are cleaner and more dependable.

My group's final project, Run and Route Hub, employs several design patterns to organize our application efficiently. MVC (Model-View-Controller) best captures the essence of our architecture. The Controller manages data flow and application logic via API route handlers, the View uses React and Next.js to render dynamic and interactive interfaces, and the Model (Prisma) defines and organizes our data structure. These elements work together to produce a modular architecture that promotes maintainability, clarity, and collaboration.

Beyond streamlining development, using MVC aligns our project with industry standards. This structure ensures contributors can work effectively within a clear framework and prepares the project for future growth.

In future projects, I will definitely be open to learning and implementing other design patterns and exploring how their concepts can apply to systems beyond programming.

## Conclusion

ICS 314 has been a formative experience. Functional programming gave me tools to write cleaner and more predictable code. Coding standards taught me how to collaborate effectively and avoid simple mistakes.Lastly, design patterns provided architectural principles that make systems scalable and maintainable. Together, these lessons changed how I approach software problems.

Moving forward, I will continue to apply these practices in both academic and personal projects. I plan to: 

- Use functional patterns where appropriate to make code easier to reason about.
- Enforce linting and formatting in team projects to improve collaboration.
- Choose design patterns deliberately to balance clarity and flexibility.

To develope something meaningful, passionate, and screams me.