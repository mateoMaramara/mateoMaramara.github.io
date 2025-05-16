---
layout: project
type: project
image: img/manoa.png
title: "ManoaConnect"
date: 2025
published: false
labels:
  - C
summary: "Manoa Connect is a centralized platform for students at the University of Hawai‘i at Mānoa to explore clubs, connect with communities, and manage their campus involvement. The Club Hub system allows students to browse club profiles, view posts, and use dashboards to manage participation. Club leaders can create or manage club entries, while admins can remove inappropriate content."
---
<img width="600px" class="rounded float-start pe-4" src="../img/connect.png">

ManoaConnect
Brief Overview
ManoaConnect is a full-stack web application built by our team for ICS 314: Software Engineering at the University of Hawaiʻi at Mānoa. Our goal was to create a centralized platform for students to discover clubs, events, and support services tailored to their interests and academic backgrounds. The platform includes a personalized dashboard, club discovery tools, admin features for student organizations, and a "Need Help?" section for accessing campus resources. We designed it to improve student involvement and reduce friction for both users and club leaders.

My Contributions
I was primarily responsible for all things database in this project. Because I was the only one on the team with a paid Vercel account, I had exclusive access to manage our hosted PostgreSQL database and was responsible for ensuring that the back end functioned properly across development and production environments.
1. Prisma Schema Design
I created and maintained the prisma.schema file, which defined all the models and relationships in our database, including Clubs, Users, Posts, and Tags. This schema was the foundation of our app’s data logic, and I iterated on it to support our growing feature set.
2. Seed Data & Environment Configuration
I developed the seed.ts script to populate our database with sample data for development and testing. This made it easier for the team to visualize how the app should look and behave. I also handled configuration through settings.development.json to ensure proper connections with our remote database on Vercel.
3. Club Data Read/Write Operations
I built out the entire read and write functionality for our Clubs component. This included retrieving and displaying club listings on the frontend, creating new clubs through form submissions, editing club data, and deleting records. All of this required careful integration between Prisma queries and React components.
4. Logo Design and Branding
I used ChatGPT to generate multiple logo concepts for ManoaConnect. After reviewing several iterations, our team chose one of the AI-generated designs as the final logo. It gave our project a clean, recognizable brand to match the polished UI.
5. Debugging and Deployment Support
Because I had full access to the Vercel project and the database, I managed database deployments, resolved schema conflicts, and helped teammates troubleshoot connection issues. I also supported merging and deploying features without breaking production.

What I Learned
Working on ManoaConnect showed me just how critical backend infrastructure is to a successful web app. I learned how to structure a real database using Prisma, configure live environments through Vercel, and maintain database stability while multiple teammates were pushing changes.
I gained a much deeper understanding of:
Schema modeling with relations and constraints


Environment-specific configuration


The full cycle of seeding, querying, and updating data


Handling merge conflicts and deployment blockers


It also helped me grow as a team contributor. While I often prefer working independently, this project showed me the value of collaboration. I was able to support my teammates by owning a key piece of the stack and ensuring the database layer stayed solid throughout.

---
[URL to repository](http://github.com/mateoMaramara/heartRateCalculator)
