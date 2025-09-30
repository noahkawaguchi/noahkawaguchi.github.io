# CSPB 3112 Project Proposal

This project is a full stack web app with the backend in Rust (Axum) with PostgreSQL and the frontend in TypeScript (React). There are users, friendships, and posts, with the twist that all posts must be in response to another post, creating a tree structure from the single root post. I have an existing codebase that I will be expanding upon this semester.

## Vision Statement

This project will allow me to gain a better grasp of both the technical knowledge and conceptual frameworks needed to effectively build web applications. While the primary focus will be on backend development, I will also gain valuable knowledge and experience in frontend development and other core aspects of software such as deployment and documentation.

## Motivation

My motivation for building a full stack web app in this project is that I would like to pursue a career in software engineering focusing on backend web development. This is also my motivation for choosing technologies such as TypeScript/React, PostgreSQL, and Docker/AWS—they are widely used in industry.

My motivation for choosing Rust (Axum) is slightly different. While Rust is growing in popularity in general and in backend development specifically, it is certainly not as common as languages like Python and TypeScript in this area. However, I have a significant amount of Rust already written for this project, so expanding from what I have will allow me to encounter more new concepts than I would if I started over using a different language. Also, Rust’s strong static guarantees and straightforward tooling allow me to focus my learning on questions of functionality and design independent of the specifics of any language or framework.

## Specific and Measurable Goals (Learning Objectives)

Backend design: While a completely thorough study and application of Domain-Driven Design and/or Hexagonal Architecture is out of the scope of the semester, the backend’s design should move in that direction. Specifically, the user, friendship, and post domains should be isolated from each other, and infrastructure such as PostgreSQL should be separated from the app’s core.

Testing: In the backend, all handler functions should be tested. (Other layers already have relatively good coverage.) In the frontend, a few key areas currently have tests, but coverage is much lower than the backend. The frontend test coverage should be increased as time allows, but not at the expense of the backend, as this is a backend-focused project. Any new features added should be tested as well.

Features: Users should be able to edit, archive, and delete posts, as the current post creation rules depend on these unimplemented features. Less critically, users should also be able to delete/modify their account and unfriend people.

Deployment: The frontend and backend should both be deployed in some capacity. The frontend can be on GitHub Pages, which is relatively straightforward. The backend should ideally be Dockerized on AWS.

Documentation: The current rather minimal README should be expanded to include explanations of concepts and approaches used in the project and demonstrations of key features. If time allows, the app itself should include some kind of demo or sandbox mode so that users don’t need to make an account to try out its functionality.

## Risks to Project Completion

Since I am not starting from scratch, the core technologies from which the project is built are less of a risk. However, as the project continues to expand, the scale and concepts I encounter move further from coursework and other personal projects I have done. Therefore, I would say the main risk is not properly grasping the scale of the various goals of the project before taking them on.

For example, while I technically do currently have a different project successfully deployed to AWS, I feel like I barely made it work, and I used a different set of their services than I would for this project. Therefore, the deployment step might end up being a more extensive task than I expect.

## Mitigation Strategy

My mitigation strategy will be keeping an open mind to changing direction. If a task at hand is taking more time than expected, I’ll reevaluate whether I need to take a step back and replace it with a more pragmatic approach that would achieve a similar result.

Continuing with the AWS deployment example, if I find that my planned deployment strategy is too time consuming or out of the scope of the semester, I could switch to a simpler option like Render or Railway.

## Project Assessments

While there is always more than can be added to this kind of project, my criteria for considering this semester’s work completed are generally the same as completing the goals listed above. As a bare minimum, the current redesign of the backend should be completed, the backend should be fully tested, and both frontend and backend should be deployed.

## Project Portfolio Link

https://noahkawaguchi.github.io/

