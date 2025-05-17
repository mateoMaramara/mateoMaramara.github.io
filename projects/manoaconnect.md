---
layout: project
type: project
image: img/logo.png
title: "ManoaConnect"
date: 2025
published: true
labels:
  - React
  - Bootstrap 5
  - Next.js
summary: "Manoa Connect is a digital platform that connects UH Mānoa students with registered independent organizations based on their interests and academic background."
---
<img width="800px" class="rounded float-start pe-4" src="../img/connect.png">

<div style="clear: both;"></div>

### My Contribution:
My primary role in the ManoaConnect project was designing and managing the database. The role entailed ensuring all of the club and user data could read and write to the vercel database. Since I was the only team member with a Vercel pro account, I had to make sure all of the user data was correctly writing to the database. This made me responsible for backend schema design, database seeding, migrations, and live data connectivity.

---

### Prisma Schema
I built the foundational schema for our app using schema.prisma. This file defined our models—like Club, User, and Post—and handled relations and constraints. For example, here’s the Club model I defined:

<img width="800px" class="rounded float-start pe-4" src="../img/schema.png">

model Club {
  id          Int      @id @default(autoincrement())
  name        String
  description String
  creator     String
  email       String
  image       String
  createdAt   DateTime @default(now())
}


### Read/Write Operations
I implemented full CRUD functionality for Clubs using Prisma and Next.js API routes. This allowed users to:
create new clubs and remove old clubs.


Here’s an example of how I created a new club:
export async function makeClub(club: {
  name: string;
  description: string;
  creator: string;
  email: string;
  image: string;
}) {
  await prisma.club.create({ data: { ...club } });
}

---

### Query Parameters and Navigation
To keep performance high and eliminate redundant API calls, I coordinated with frontend developers to use query parameters instead of repeated backend requests. This allowed data like club name, email, and image URL to be passed via the URL using useSearchParams() and the router.push() method.
Example:
const searchParams = useSearchParams();
const name = searchParams.get('name') || 'Unnamed Club';

This strategy allowed us to pass club data between pages without needing to re-fetch it, improving load time and the overall user experience.

---

### Logo Design Using AI


In addition to backend responsibilities, I also contributed to the branding of the project. Using ChatGPT, I generated multiple logo concepts for ManoaConnect. After reviewing several options, the team chose one of the AI-generated designs as the final product, which we used across our site for consistent visual identity.

### What I Learned
Through this project, I gained deep, practical experience in full-stack web development with a strong focus on the backend and deployment pipeline. Here’s what stood out most:
Database Design with Prisma: I learned how to define and enforce structured data models using schema.prisma, connect them to the frontend, and use them safely in production.


Seeding and Environment Management: I gained hands-on experience with writing seed.ts scripts and configuring .env and development JSON files for remote PostgreSQL databases hosted on Vercel.


Backend Integration with React & Next.js: I bridged backend and frontend logic with well-defined API routes, enabling smooth form submission and dynamic content loading.


Query Parameters for Efficiency: I saw the benefits of using query strings for state transfer across pages, saving time and database bandwidth.


AI-assisted Branding: I creatively applied ChatGPT for logo design, giving our project a clean and cohesive identity.



### Conclusion

ManoaConnect gave me the opportunity to lead critical backend development and become comfortable working in a full production environment. I learned how to keep a team project stable by owning a key part of the stack, and I became more confident handling real-world database tasks that extend beyond the classroom. This experience has made me more prepared for industry-level backend development and has sharpened my understanding of full-stack architecture.


---
[URL to repository](https://manoaconnecttb.github.io/)
