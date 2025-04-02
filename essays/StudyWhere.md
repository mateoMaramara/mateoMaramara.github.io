---
layout: essay
type: essay
title: "Final Project Idea"
# All dates must be YYYY-MM-DD format!
date: 2025-04-01
published: true
labels:
  - Software Engineering
  - Nextjs
---
<img width="400px" class="rounded float-start pe-4" src="../img/vs.png">
## Overview

### The problem:
UH Mānoa students often struggle to find quiet, available, or well-equipped places to study on campus. Library seating is limited, lounges are noisy, and there's no reliable, real-time way to check conditions before showing up. Students waste time walking around campus trying to find the “right vibe” for studying — quiet, well-lit, with outlets and decent Wi-Fi.

### The solution:
**StudySpace UH** is a crowdsourced study spot finder designed for the UH Mānoa campus. Students can log in and view a live map of study locations, updated with user-submitted conditions like noise level, crowd density, outlet availability, and Wi-Fi reliability. Users can submit quick feedback about where they’re studying, helping others find ideal spots in real time. Users can also save their favorite spots and get personalized suggestions based on time of day, past preferences, and proximity.

## Approach

StudySpace UH has three user roles:

- **Regular users** log in with UH credentials to view and contribute live study space reports. They can set preferences (quiet vs. busy, indoor vs. outdoor, etc.) to get personalized suggestions.
- **Moderators** can review flagged posts or inappropriate reports and remove or edit inaccurate content.
- **Super Admins** can add new study locations, update maps, and promote moderators.

The site goes beyond a static list — it includes filtering and sorting options, such as:
- Noise level (quiet, moderate, noisy)
- Seating availability (low/medium/high)
- Wi-Fi strength
- Time of day recommendations
- Map view and list view

### Special Sauce
Each user has a **personalized dashboard** that suggests study spots based on their preferences, location, and past activity. Returning users can “favorite” locations and get custom suggestions when spots are reported full or too loud.

## Proposers
This idea was collaboratively developed by:
- Mateo Maramara

## Mockup Pages
- **Landing Page**: Clear branding and explanation of the app, plus login portal
- **Dashboard**: Personalized user view with suggested study spots, favorite spots, and quick-submit buttons
- **Live Map Page**: Interactive map with real-time pins and filters
- **Submit Report Page**: Easy UI to quickly submit a spot condition update
- **Admin Panel**: For moderators and super admins to manage data

## Use Case Ideas
- **Jasmine**, a nursing major, logs in between classes and gets three recommended quiet spots with outlets and AC.
- **Marco**, a night owl, sets his preferences for “low traffic, outdoor spots” and receives notifications when the Hamilton Library patio area becomes available.
- **Daniel**, a moderator, removes a report that falsely labeled a spot as “silent” when it was next to a concert rehearsal.
- **Leilani**, a first-year student, discovers the Sinclair Building second floor is consistently rated “best evening vibe” and favorites it for future sessions.

## Beyond the Basics
Future enhancements might include:
- Integration with campus Wi-Fi metrics to auto-report connectivity strength
- Heatmap overlay based on recent crowd reports
- AI-based prediction of best future study spots by time/day
- Badge system for reliable reporters (like Yelp Elites)

