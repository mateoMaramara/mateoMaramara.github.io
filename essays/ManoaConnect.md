---
layout: essay
type: essay
title: "Final Project Idea"
date: 2025-04-01
labels:
  - Software Engineering
  - Nextjs
---

## Overview

### The Problem:
At UH Mānoa, many students feel disconnected from campus life and don’t know how to get involved in extracurriculars. While there are over 200 Registered Independent Organizations (RIOs), participation is low, especially among new and transfer students. Existing tools like club lists or newsletters are fragmented, outdated, or hard to navigate.

### The Solution:
**CampusConnect** is a personalized digital platform that helps UH Mānoa students discover clubs, events, and academic support tailored to their interests. After logging in with a UH email and completing a short onboarding quiz, users receive a custom engagement feed showing upcoming events, relevant student orgs, and support services (like the Writing Center or Learning Emporium). Organizations can manage content through a dedicated admin portal.

This platform combines personalized recommendation logic, modern UI/UX, and campus-focused features to strengthen student belonging and community engagement.

## Approach

CampusConnect includes multiple user roles:
- **Students** log in with a UH email and receive a personalized dashboard based on their major and interests.
- **Organization Reps (6 per org)** can log in and manage announcements, events, and posts.
- **Super Admins** moderate content, approve new clubs, and assist with onboarding new orgs.

### Key Functional Pages:
- **Landing Page**: Overview of CampusConnect + login
- **Quiz Page**: Choose majors, interests, and preferred engagement types (academic/social/etc.)
- **Home Dashboard ("For You")**: Personalized feed of events, posts, and opportunities
- **Explore Tab**: Browse/search organizations by tags (e.g., “STEM,” “Social Impact,” “Athletics”)
- **Admin Portal**: Club accounts can manage posts and view engagement stats

## Special Sauce
The personalization engine is the "special sauce" — no two users see the same dashboard. Feed content is generated based on quiz answers and user behavior. Organizations also get feedback on which demographics are interacting with their content, helping them better target and connect with students.

## Proposers
This idea was collaboratively developed by:
- Mateo Maramara, Computer Science
- Michael Peterson, Computer Science
- Laurent Keith Villanueva, Computer Science

## Mockup Pages
- **Landing Page** – Welcome message, how it works, UH email login
- **Quiz Page** – Majors, interests, engagement types
- **Dashboard Page** – Personalized feed ("For You")
- **Explore Page** – Browse/search orgs and events
- **Org Admin Page** – Create/manage posts, view engagement
- **Need Help? Page** – Quick access to campus services (Writing Center, Learning Emporium, etc.)

## Use Case Ideas
- **Keoni**, a first-year Biology student, takes the quiz and gets matched with 5 clubs, including a hiking club and pre-health org.
- **Sarah**, an English major with an interest in Filipino culture, finds a student org that she wouldn’t have discovered otherwise.
- **Justin**, a club officer, logs in to schedule a post and upload a flyer for an upcoming social event.
- **Transfer student** Hana checks her dashboard and finds academic support resources she didn’t know existed.

## Beyond the Basics
- **Real-time event reminders and RSVP integration**
- **Analytics dashboard** for organizations
- **Badging system** for highly involved students
- **Potential API integration** with UH systems (STAR, campus calendar)
- **Expansion-ready** architecture to support other campuses

