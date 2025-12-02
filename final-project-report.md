# Final Project Report

## Introduction

My vision for this project was to expand my knowledge and abilities in creating full stack web apps. Expanding an existing codebase, I aimed to learn about concepts, issues, and methodologies that I could only encounter by reaching a larger scale than I had in previous personal projects.

This vision included specific goals in various areas. I wanted to make the backend design more decoupled, testable, and maintainable. I wanted to increase test coverage across the stack and implement several new features. I wanted to deploy both backend and frontend and expand the project's documentation.

## Background

While on the surface, the project is a social media app with a twist, the actual significance of the project is the depth to which I was able to gain experience with web app technologies. My most significant previous project used AWS Lambda and DynamoDB and did not have any kind of user accounts or login. In contrast, the project I worked on in this course uses more generally applicable technologies such as a regular HTTP server, PostgreSQL, and Docker, and it fully includes user authentication with bcrypt hashing and JSON Web Tokens.

Consequently, this project proved to be very beneficial to my professional development. I now have a much clearer understanding of many of the standard tools and approaches used in web apps. As I worked on the project throughout the semester, I not only became more comfortable with the development workflow, but also had the opportunity to experience for myself why some of these tools and approaches are used. For example, after completing the Docker stage of the project, I was able to run my entire backend stack in different environments with ease.

## Methods and Materials

Since I was not starting from scratch at the beginning of the semester, I already had a lot of the foundational knowledge and skills required. However, there were still many new concepts I had to familiarize myself with in order to make informed decisions and achieve my goals.

The main process that I used to achieve this was having AI teach me rather than do things for me. I found that general tutorials almost never cover quite what I need to learn to achieve the task at hand. Of course, just having AI generate some solution without understanding it does not help me learn anything, and is almost always not quite what I need anyway. Whenever I needed to learn a new concept to progress in the project, I would start with a general prompt and then gradually ask more specific questions as I expanded my understanding. I also made sure to ask from some different angles and compare the results with some more "deterministic" sources like GitHub READMEs to make sure I was not blindly following inaccurate information. As I deepened my understanding of a particular topic, I would also spend a good deal of time reading documentation directly rather than just trusting that AI-generated code is up to date and appropriate for my use case.

I found this process to be greatly successful overall, and I feel like I solidly learned the concepts that I approached in this way. One potential area for improvement is that I think I spent too much time delving into details. When striking a balance between maintaining a deep understanding of what is going on and trusting AI to be close enough, I think I could have been more efficient overall if I had let go a bit and allowed my understanding to stay at a slightly higher level.

## Results

I would say that what I learned falls into four categories: high-level concepts, commonly used tools, less commonly used tools, and my own preferences.

In arguably the most important category, high-level concepts, I encountered various software engineering topics firsthand. For example, some modules were dependent on others' concrete implementations rather than abstractions, complicating testing. In other cases, the boundaries between service and repository layers were unclear, creating trade-offs between separation of concerns and avoiding race conditions. I was able to solve both of these issues by decoupling dependencies using traits (interfaces) that integrate with transaction logic where appropriate.

In terms of tools, some of the ones I learned are more popular than others, but I feel like I got a lot out of all of them. For example, Docker, Docker Compose, and AWS are increasingly essential skills regardless of programming language. I was also able to get much more comfortable with using workflow-related tools in a more professional way. Namely, I used branches, issues, pull requests, and GitHub Projects (kanban boards) in a very structured way that resembled collaborative work.

On the other hand, I used some less broadly known utilities like Atlas (for database migrations) and Caddy (for HTTPS) for the first time in this project, and they ended up helping me solve key problems relatively easily. I would say that I struck a good balance between learning tools that are broadly used and tools that are less popular but solve problems specific to the project.

Finally, I learned a lot about my interests and abilities, which I explain in more detail in the conclusion.

I know that I learned these things mostly because of the results of what I created. I am not a complete expert at anything I learned yet, but I have a clear understanding of the motivation behind essentially all of the decisions that make up the project. I would say that what I have been able to create is not perfect, but solidly demonstrates knowledge of the topics I learned.

My project assessments were primarily to complete my stated goals. I set redesign, testing, and deployment as a bare minimum, which I achieved. Of the other goals, the only one I decided to forgo was features, as explained further in the next section.

## Discussion and Reflection

I met all goals except the one regarding feature expansion. Several factors contributed to this success. One key point was that I already had a significant amount of work done on the project, and was expanding it this semester rather than starting with a blank slate. This allowed me to more accurately estimate the scope of various tasks. However, many tasks were still new to me and relatively difficult to gauge beforehand. I handled this by adapting my strategies to stay within the scope of the semester while still fulfilling the terms of my initial goals. For example, for my AWS deployment, I explored RDS and App Runner, but decided to go with plain EC2 instead. I had also given myself the further fallback of not even using AWS, and even though I ended up successfully using AWS, that kind of flexible mindset was important to achieving my goals. Along the same lines, I was able to achieve most of my goals by leaving out one of them, feature expansion. Since this would have covered much of the same conceptual territory that I had already explored, I decided to prioritize unfamiliar areas to focus on learning the new concepts that I wanted to learn.

I feel very positive about the project results. Definitely in general terms, and even for the most part in specific terms, I achieved exactly what I said I would. As discussed in the results section, I learned a lot of important concepts relating to both core skills and specific interests.

## Conclusion

This project was an extremely important part of my professional development and provided me with many insights into potential career directions to pursue. While learning about specific technologies was one major benefit, I was also able to reflect on what I did and did not feel was a good fit for me.

Leading up to and including this project, I have focused on building full-stack web apps because that is the "default" personal project type and professional direction. However, as I explored this area more deeply in this project, some doubts I had been feeling before became more prominent. I have now done a good number of projects with TypeScript/React/Vite frontends, and I thought that with experience, I might learn to like or at least tolerate this stack. However, if anything, I have been disliking it even more, both in terms of the specific tooling and broader frontend concepts. If I make another web app project in the future, I am thinking I will explore a template-based approach rather than a backend API and separate frontend, but even then, I doubt that is a solution to the fundamental issue.

One key clue toward the broader career takeaways from this project is my choice of Rust for the backend and my experience of using it throughout the project. In more specific terms, I can tolerate and even enjoy a language having relatively higher conceptual complexity, especially when it is helping me carry out my intentions in a very precise way, but expect tooling to be cohesive and straightforward. I found that most of the difficulty of Rust is working with its distinctive system of ownership, borrowing, and lifetimes, while most of the difficulty of TypeScript and Node is debugging configuration files, tooling incompatibilities, and unintuitive library code behavior.

Going beyond a direct comparison of two languages, I think these findings reflect broader differences in the fit of potential professional directions. Even though I only used TypeScript in the frontend in this project, I have had similar experiences in the past with backend TypeScript and Python. When it comes to the general problem of implementing a high level business idea as a web app, it makes sense to me that resolving issues with configuration, tooling, libraries, and frameworks would be one of the most important skills, while using a language with more precise control and conceptual overhead as I did in the backend portion of this project is unnecessary or even a liability.

Consequently, I am considering trying to move away from web apps in hopes that I will find something more in line with my approach to problem solving. Regardless, this project proved to be immensely helpful by giving me a lot of context and experience that will help guide me moving forward.

## References

As mentioned above, pretty much all of the learning materials that ended up having some impact on what I created were either official documentation or AI generated, so I do not really have anything to list such as online courses or academic articles. As for my products, the main results that I have are the deployed project itself, its GitHub repository, and the weekly posts documenting the process. Smaller products such as the kanban board and Docker image are also accessible from the repository.

Deployed URL: [spur.noahkawaguchi.com](https://spur.noahkawaguchi.com)

Repository: [github.com/noahkawaguchi/spur](https://github.com/noahkawaguchi/spur)

Posts: [noahkawaguchi.github.io](https://noahkawaguchi.github.io)
