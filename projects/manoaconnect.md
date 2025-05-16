---
layout: project
type: project
image: img/manoa.png
title: "ManoaConnect"
date: 2025
published: true
labels:
  - React
  - Bootstrap 5
  - Next.js
summary: "Manoa Connect is a centralized platform for students at the University of Hawai‘i at Mānoa to explore clubs, connect with communities, and manage their campus involvement. The Club Hub system allows students to browse club profiles, view posts, and use dashboards to manage participation. Club leaders can create or manage club entries, while admins can remove inappropriate content."
---
<img width="600px" class="rounded float-start pe-4" src="../img/connect.png">

ManoaConnect

My Contribution: Database Design, Integration, and Club Functionality
My main role in the ManoaConnect project was designing and managing the database, ensuring that all club-related data was modeled correctly, stored securely, and retrieved efficiently. Since I was the only team member with a paid Vercel account, I was also the only one who could manage the hosted PostgreSQL database used in development and deployment. This made me responsible for backend schema design, database seeding, and live data connectivity.

1. Prisma Schema Design
I built the foundational schema for our app using schema.prisma. This file defined our models—like Club, User, and Post—and handled relations and constraints. For example, here’s the Club model I defined:
model Club {
  id          Int      @id @default(autoincrement())
  name        String
  description String
  creator     String
  email       String
  image       String
  createdAt   DateTime @default(now())
}

This schema made it possible for us to structure and enforce how data flows through the app, and how it's queried and mutated via Prisma.

2. Seeding and Configuring Development Environments
I created the seed.ts script to populate the database with example entries for clubs, helping our team test and demo the app with real-looking data. I also managed settings.development.json and other configuration files to ensure our local and deployed apps were properly connected to the remote PostgreSQL instance hosted by Vercel.

3. Read/Write Club Operations
I implemented full CRUD functionality for Clubs using Prisma and Next.js API routes. This allowed users to:
Create a new club with metadata


Read from the club list and individual profiles


Edit club information


Delete entries when necessary


Here’s an example of how I created a new club on the backend:
export async function makeClub(club: {
  name: string;
  description: string;
  creator: string;
  email: string;
  image: string;
}) {
  await prisma.club.create({ data: { ...club } });
}

This function was linked to our Create Club form and handled the entire backend logic for club creation.

4. Query Parameters and Navigation
To keep performance high and eliminate redundant API calls, I coordinated with frontend developers to use query parameters instead of repeated backend requests. This allowed data like club name, email, and image URL to be passed via the URL using useSearchParams() and the router.push() method.
Example:
const searchParams = useSearchParams();
const name = searchParams.get('name') || 'Unnamed Club';

This strategy allowed us to pass club data between pages without needing to re-fetch it, improving load time and the overall user experience.

5. Logo Design Using AI
In addition to backend responsibilities, I also contributed to the branding of the project. Using ChatGPT, I generated multiple logo concepts for ManoaConnect. After reviewing several options, the team chose one of the AI-generated designs as the final product, which we used across our site for consistent visual identity.

What I Learned
Through this project, I gained deep, practical experience in full-stack web development with a strong focus on the backend and deployment pipeline. Here’s what stood out most:
Database Design with Prisma: I learned how to define and enforce structured data models using schema.prisma, connect them to the frontend, and use them safely in production.


Seeding and Environment Management: I gained hands-on experience with writing seed.ts scripts and configuring .env and development JSON files for remote PostgreSQL databases hosted on Vercel.


Backend Integration with React & Next.js: I bridged backend and frontend logic with well-defined API routes, enabling smooth form submission and dynamic content loading.


Query Parameters for Efficiency: I saw the benefits of using query strings for state transfer across pages, saving time and database bandwidth.


AI-assisted Branding: I creatively applied ChatGPT for logo design, giving our project a clean and cohesive identity.



Conclusion
ManoaConnect gave me the opportunity to lead critical backend development and become comfortable working in a full production environment. I learned how to keep a team project stable by owning a key part of the stack, and I became more confident handling real-world database tasks that extend beyond the classroom. This experience has made me more prepared for industry-level backend development and has sharpened my understanding of full-stack architecture.


---
[URL to repository](http://github.com/mateoMaramara/heartRateCalculator)
