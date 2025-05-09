---
layout: essay
type: essay
title: "Artificial Code"
# All dates must be YYYY-MM-DD format!
date: 2025-04-23
published: false
labels:
  - Design
---

<img width="500px" class="rounded float-start pe-4" src="../img/robot.webp">

I. Introduction
Artificial Intelligence (AI) is one of the most transformative tools in software engineering today. In education, it plays a growing role—from correcting syntax and suggesting completions to explaining abstract concepts in natural language. In ICS 314: Software Engineering, I used AI tools like ChatGPT and GitHub Copilot extensively. Whether I was working with TypeScript, React, Next.js, or Prisma, these tools provided support in understanding, debugging, and writing code. Rather than relying on AI for shortcuts, I treated these tools as scaffolding for deeper learning and mastery.

II. Personal Experience with AI
1. Experience WODs (e.g., E18)
For Experience WODs that lacked video solutions—or when walkthroughs didn’t match my specific implementation—I often turned to ChatGPT. One example was during a WOD involving sorting posts by creation date in a Prisma query. I encountered the error:
“Object literal may only specify known properties, and 'createdAt' does not exist in type 'PostOrderByWithRelationInput'”
 I asked:
 “What does this Prisma error mean and how can I fix it?”
 ChatGPT explained how Prisma's type-safe API required createdAt to be defined properly in the schema. It also walked me through how to check the generated types and correct the query. This real-time explanation helped me finish the WOD correctly without waiting for external help.

2. In-Class Practice WODs
I frequently used AI during Practice WODs to clarify concepts and strengthen my understanding before timed in-class sessions. For example, while preparing for a Practice WOD involving form submission and TypeScript props, I asked:
“How do I fix this error: ‘Expected 1 arguments, but got 0. ts(2554)’ when calling a function in a React form?”
 ChatGPT helped me realize that my event handler was missing an argument (event), and it explained how to properly type and pass event objects in TypeScript. That insight made React’s event system more intuitive and helped me avoid preventable runtime issues later on.

3. In-Class WODs
In-class WODs were the most stressful because they were timed and often included a twist on the Practice WODs. One example involved working with Prisma queries, where I encountered a TypeScript type error during filtering. I asked:
“How do I fix: 'createdAt' does not exist in type 'PostOrderByWithRelationInput'?”
 ChatGPT helped me quickly understand the problem and restructure my query. Since I couldn’t always depend on AI when prompts were posted as images, this moment reminded me of how reliant I had become—and how important it was to internalize the fixes AI suggested.

4. Essays
AI was helpful for brainstorming technical concepts, but not so much for expressing my unique perspectives. For the essay on design patterns, I asked:
“Explain the Factory Design Pattern with a TypeScript example.”
 ChatGPT gave a textbook explanation, but I still needed to create my own analogy to understand and communicate the pattern. The AI provided the foundation, but the clarity came through my own effort to personalize the explanation.

5. Final Project
By the time we started our final project, I found myself relying less on AI. Many of the technical problems—like dynamic routing in Next.js or setting up relational queries with Prisma—were things I had struggled through earlier. However, Copilot was useful for small things like catching ESLint errors and suggesting cleaner syntax. For example:
“Expected indentation of 12 spaces but found 14.”
 These micro-suggestions saved time and helped keep the codebase consistent.

6. Learning Concepts / Tutorials
This was probably my primary use case for AI tools. I constantly asked questions like:
“Can you explain getServerSideProps vs getStaticProps in Next.js?”
 “What’s the best way to type a React component with props in TypeScript?”
 Rather than asking AI to complete tasks for me, I used it to help me understand concepts that were difficult to grasp from the docs alone. This built my confidence and helped me troubleshoot more independently.

7. Answering Questions in Class or Discord
I didn’t often ask questions in class or on Discord because AI tools provided faster, personalized responses. If I still couldn’t figure something out after checking AI and documentation, I’d then reach out to my classmates or professor—but AI was my first stop.

8. Asking or Answering a Smart Question
Similar to Discord posts, I didn’t formally engage in asking “smart questions” during class. Instead, I tried to answer those questions myself by experimenting and prompting ChatGPT until I could explain it clearly to myself.

9. Coding Example (e.g., .pluck in Underscore)
During ICS 314, I often used AI tools to generate quick examples when I didn’t fully understand a syntax pattern. One memorable instance was when I asked:
“Can you explain how to use arrow functions in JS and TS?”
 I had seen arrow functions used with .map() and .filter() but wasn’t sure when to include parentheses, curly braces, or return statements. ChatGPT walked me through examples showing differences between implicit and explicit returns, as well as how arrow functions behave with this. These explanations helped me confidently write functional-style array methods in several WODs and improved my fluency in TypeScript syntax.

10. Explaining Code
One of my most common uses of ChatGPT was to understand unfamiliar or broken code. I would paste a function and ask:
“Can you explain this function line by line?”
 The tool’s explanations helped me diagnose bugs more quickly and often revealed hidden logic errors that I hadn’t noticed.

11. Writing Code
I occasionally asked AI to help scaffold functions. For example:
“Write a TypeScript function that filters posts by the current user ID.”
 While I rarely copied code directly, having a structural reference made it easier to get started. Over time, I started relying less on these prompts as my confidence grew.

12. Documenting Code
I didn’t use AI for writing documentation. Instead, I wrote my own comments, both to clarify logic for teammates and to reinforce what I had learned.

13. Quality Assurance / Debugging
Whenever I hit confusing bugs, I asked things like:
“Why is this throwing a TypeError: undefined is not iterable?”
 Or:
 “How do I fix ‘Property does not exist on type Post’ in TypeScript?”
 ChatGPT would usually walk through possible causes, including checking null safety, optional chaining, or Prisma schema definitions. These were critical to resolving issues quickly under pressure.

14. Other Uses
Here are a few more examples:
During API development, I asked:


 “How do I filter a Prisma query based on a related model field in Next.js API routes?”



While building the explore page, I asked:


 “What’s the best way to display filtered search results using React state?”
 In both cases, AI helped me structure logic that I could later improve and personalize.




III. Impact on Learning and Understanding
AI tools helped accelerate my learning, especially when documentation was unclear or when I didn’t know what keyword to Google. Instead of copying code, I learned to ask “why” something worked. ChatGPT helped me understand Prisma query patterns, React lifecycle behavior, and TypeScript typing strategies that weren’t obvious in the docs. This made me a more independent and confident developer.

IV. Practical Applications
Outside of ICS 314, I used ChatGPT for job interview prep and GitHub Copilot while working on side projects. One prompt I used was:
“Create a mock API route that returns user data in Next.js.”
 This gave me a template I could adapt and understand. AI also helped me debug Vercel deployment issues related to Prisma migrations by suggesting correct CLI flags and environment variable setups. These real-world uses validated the course content and reinforced what I was learning.

V. Challenges and Opportunities
The biggest challenge was resisting the urge to overuse AI. At times, it was tempting to paste in the prompt and let Copilot write the entire function. But I realized that when I took the time to write code myself—even if it was slower—I remembered it better. A future opportunity is integrating AI literacy into the curriculum: teaching students not just how to code, but how to critically evaluate AI-generated code.

VI. Comparative Analysis
Traditional methods like reading documentation and reviewing lecture slides helped me build deep, foundational knowledge. But AI added speed, flexibility, and a low-pressure environment for asking “dumb” questions. Combining the two—traditional teaching and AI-enhanced tools—offered the best of both worlds: deep learning with real-time feedback.

VII. Future Considerations
As AI tools improve, their role in software engineering education will grow. But we need to teach ethical use, critical thinking, and prompt engineering alongside syntax and frameworks. AI should be positioned as a learning companion—not a crutch or a threat. Educators can also use AI to generate examples, design auto-feedback tools, and simulate code review sessions for students.

VIII. Conclusion
My experience in ICS 314 would have been very different without AI tools like ChatGPT and GitHub Copilot. These tools helped me understand code, debug faster, and practice independently. More importantly, they helped me grow as a learner. I wasn’t just solving problems—I was learning how to learn. My recommendation for future courses is to embrace AI, teach it responsibly, and empower students to use it not to replace thinking—but to enhance it.

Let me know if you'd like this exported to PDF, DOCX, or formatted for a portfolio page.


