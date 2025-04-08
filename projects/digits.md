---
layout: project
type: project
image: img/contact.jpeg
title: "Digits"
date: 2025
published: true
labels:
  - Next.js
  - TypeScript
  - PostgreSQL
summary: "Digits is a web application that allows users to manage their personal contacts and attach notes to them. Built with Next.js, Prisma, and PostgreSQL."
---

**Digits** is a contacts and notes management application I built as part of the ICS 314 course at the University of Hawaiʻi. Users can log in securely, add new contacts with details like name, address, image, and description, and attach notes to each contact to track interactions or personal reminders.

Each user can only see and manage their own contacts and notes, while administrators can view all users and their contacts. The app uses modern technologies including **Next.js**, **Prisma ORM**, **PostgreSQL**, and **TypeScript** to ensure scalable, maintainable, and performant development.

---

### 🖼 Screenshots

**Home Page:**

<img width="400px" class="rounded float-start pe-4" src="img/DIGIT1.PNG">

**Add Contact Page:**

<img width="400px" class="rounded float-start pe-4" src="img/DIGIT2.PNG">

**List Contact Page:**

<img width="400px" class="rounded float-start pe-4" src="img/DIGIT3.PNG">

**Add Note on Contact:**

<img width="400px" class="rounded float-start pe-4" src="img/DIGIT4.PNG">

**List Contact Page (with Notes):**

<img width="400px" class="rounded float-start pe-4" src="img/DIGIT5.PNG">

---

### 💻 Features

- 🔐 Secure login with NextAuth
- 📇 Add, edit, and delete contacts
- 📝 Attach timestamped notes to contacts
- 🧑‍💼 Admin interface to view all users and contacts
- 📱 Fully responsive with React Bootstrap

---

### 🚀 Installation Instructions

1. **Clone the repository:**

```bash
git clone https://github.com/mateoMaramara/digits.git
cd digits
