---
layout: essay
type: essay
title: "How I Utilized AI in ICS314"
# All dates must be YYYY-MM-DD format!
date: 2024-12-14
published: true
labels:
  - AI
  - Software Development
---

<img class="img-fluid" src="../img/ai/ai-header.png">

# Introduction

At the moment, the role of AI in education is huge. AI has been used to automate many mundane tasks, and can be used to gather inspiration for ideas. In software engineering specifically, AI can be used to help fill in code, think of ideas for projects, help with general software information, the possibilities are endless. The main AI tool I've made use of is ChatGPT. I typically use ChatGPT whenever I get stuck on a problem. I ask the AI for hints on how to solve the problem, instead of asking it to solve the issue outright. This is because if I rely on ChatGPT to solve all my problems for me, I won't be a good software engineer. Furthermore, ChatGPT currently isn't advanced enough to answer all my questions. Even if I ask it to do my assignment for me, chances are that it'll miss requirements, use the wrong libraries, etc.

# Personal Experience with AI

1. Experience WODs e.g. E18
  In Experience WODs, I remember asking AI how certain methods work. For example, in E18: Functional Programming, since it was my first introduction to the world of functional programming, I asked AI to explain to me the basic array manipulation methods (.map, .filter, etc.). It gave me insight in the methods, and when to use them. However, I found that it used "if" statements a lot in the functional methods, which went against the requirements.

2. In-class Practice WODs
  For in-class practice WODs, I didn't use AI. The reason why, was because I knew that these practice WODs weren't graded, so if I didn't finish, then it was no big deal. I thought it was more important for me to come to a solution on my own rather than depend on the AI to fix my problems for me.

3. In-class WODs

For in-class WODs, I usually didn't use AI tools. I tried to solve the WOD by myself using old resources and previous example websites. However, when I did use AI, it was typically in reference to fixing a stylistic issue. For example, I would ask it how to left-center the text in the Aloha Beer React WOD.

4. Essays

For essays, I haven't used AI. This is mainly in part due to me wanting to improve my writing skills as a software engineer. I know that AI can be a helpful tool for writing (or even writing the whole essay), but I want to make sure that my own personal voice is heard, rather than a machine-generated one.

5. Final project

In the final project, I used AI when I ran into a few problems. An example of a problem would be related to the Yup resolver. Since I never used Yup validation before, I ran into a lot of problems when trying to validate the input fields. This made me have to look into the Yup documentation and ask AI the best solution to the problems I encountered (like submitting an array of Strings, or using conditionals since some validation formats can be either null, undefined, or have a value).

6. Learning a concept / tutorial

I used AI whenever I learned a new concept. This is because I knew that AI was able to teach concepts in a simplified way, rather than throwing all the information available to me. Although I used a couple times in ICS314, I found myself using it a lot in ICS311, for questions surrounding graphing, trees, computer graphics, FFT, etc.

7. Answering a question in class or in Discord

When answering a question in class, I did not use AI. This is because it sort of felt like cheating. If I used AI to answer the professor's question, then I feel like I didn't gain anything out of it. The reasons why the professor asks questions in class is to make sure we understand the material, not test our ability to ask a chatbot then spit out the answer.

8. Asking or answering a smart-question

I haven't answered any smart-questions in the Discord yet. However, if I did, then I would first try to answer the question myself, then if I couldn't find a suitable answer, I would ask AI.

9. Coding example e.g. “give an example of using Underscore .pluck”

I have used AI for coding examples a lot. I remember asking it once to give me an example of sorting an array of objects by property. The AI gave me a reasonable example of using the .sort() method, giving me insight in how to apply it to my own problems.

10. Explaining code

I used AI to explain code to me many times. For example, I would paste in a block of code from my final project, and ask it to explain to me how it worked. Since a lot of the code came from the nextjs-application-template, it was all pre-written with no comments. This made it difficult to know what each function did, but after getting AI to explain it to me, I think I understood it better.

11. Writing code

I haven't used AI to explicitly write code for me. This is because I feel that if I ask AI to write a portion of code for me, then I copy and paste it into my assignment, I feel like I didn't learn anything. I want to be able to have the satisfaction of applying what I learned to my assignments, not just asking ChatGPT to answer it for me, and copy and paste it and pass it off as my own work.

12. Documenting code

Most documentation of the code I written was by me. Since I understand the code the best and the use cases for the code, I think I would have a better idea of how to write comments or documentation. Since AI wouldn't get the full picture, I feel like it would miss out on a lot of details.

13. Quality assurance e.g. “What’s wrong with this code..." or “Fix the ESLint errors in...”

I remember pasting in a few blocks of code and asking ChatGPT what was wrong with it. Typically, ESLint errors are simple to fix, so I wouldn't need to rely on AI for those. However, for code with logical errors or syntactic errors, GPT would be helpful in detecting those. For example, although this isn't necessarily code, I asked ChatGPT to troubleshoot why Prisma would throw an error stating "failed to apply migrations" whenever I ran prisma migrate dev. ChatGPT explained that it happens when the local database schema doesn't match the migration history, so it suggested to run "npx prisma migrate reset", then "npx prisma migrate dev".

14. Other uses in ICS 314 not listed


I believe the previous 13 points covered all my use cases of AI in ICS314.

# Impact on Learning and Understanding

Using AI in ICS314 has made a big impact on my comprehension, skill development, and problem-solving abilities. This is because AI tools like ChatGPT give immediate feedback and explanation, which help me understand complex concept more easily. Prisma and React hooks are two examples of technologies that I was unaware about, but ChatGPT was able to explain and simplify the documentation while giving real-world examples. However, there are definitely opportunities for AI to improve, since when I'd ask it for help on a complex issue, it wouldn't have a full understanding of the topic. This is understandable since it doesn't have a full grasp of the minute details of an assignment, so I used AI more as a supplementary tool rather than one to use to copy and paste from.

# Practical Applications

Outside of ICS314, I used AI to give me example topics for my group assignments in ICS311. There were times when it came to an assignment and I was sort of clueless when it came to how to organize the project. Since I was typically the group leader when it came to the weekly assignments, I would lay the groundwork for how the projects would be completed. This is where I asked AI how to start the project, and for ideas on data structures depending on the assignment guidelines. Albeit I didn't copy word-for-word from ChatGPT and didn't use copy its ideas outright, rather I took the ideas as inspiration for starting the group assignments. It was definitely helpful in getting the assignments off the ground and gathering input from my teammates on how the assignment should be written.

# Challenges and Opportunities

A challenge I've iterated in this essay over and over again, is that AI typically doens't understand the full picture when it comes to answering questions. It can't think in complex terms, and if I give it many requirements, it'll typically ignore a couple requirements and give me an answer that was totally wrong. I remember one of the teammates for my ICS314 project use an AI generator for one of the components, but was questioning why it wasn't working. When I came around to look at the code, I realized AI generated the component mostly correctly, but was using JS's fetch API to call the database. We never used this library, so it was bound to introduce errors. I replaced the database calls with the right methods and it worked.

# Comparative Analysis

When it comes to traditional teaching and AI-enhanced approaches, there are definitely a few pros and cons to each. When thinking about AI-enhanced teaching, it might be easier for the students to gain instant feedback to their questions. Also, for students who have a hard time asking questions in-class and in-person, might find it more comfortable to type out the question to a chatbot. However, the issue lies in that AI might not be 100% accurate. This is where traditional teaching shines, because the professors have decades of experience in their fields. They can also answer tailored questions about specific topics, and even provide better support than what ChatGPT can. To gain a deeper understanding of a topic, I would definitely trust my professors more than ChatGPT or any AI tool.

# Future Considerations

The role of AI in software engineering education will only continue to grow as technology advances. AI can take a role as a personalized tutor, adapting to personal learning styles and provide customized challenges, explanations, and resources for each student. Moreover, there have been tools like GitHub Copilot and integrations of AI with ESLint to help with real-time performance analysis. This can further help with improving code quality and providing a standard for how code should be written. Of course, this has the potential to lead to an over-reliance on AI for problem solving. Instead of using their own heads, the students could rely on AI too much. In addition, AI might not be the most up-to-date, causing the student to learn outdated methods to solve problems.

# Conclusion

All in all, I think the use of AI in ICS314 has been a great addition to my toolbox. It has helped me with writing code, analyzing it for errors, and providing me with ideas for projects. The integration of AI in future courses could be improved by ensuring that students don't rely on AI too much, and by encouraging the usage of AI in in-class WODs but emphasizing the fact that the students have to also understand the material.