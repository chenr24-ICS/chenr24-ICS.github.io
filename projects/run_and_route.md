---
layout: project
type: project
image: "img/M2/M2Profile.png"
title: "UH Run and Route Hub"
date: 2025
published: true
labels:
  - Software Engineering
  - React
  - Next.js
  - Typescript
  - PostgreSQL
  - CSS
  - Vercel
summary: "Team-developed web application for runners to log, access, and review running routes across Oahu"
---

# Overview

**Run & Route Hub** is a running-focused web app for UH students that helps runners:

- Find running partners based on pace and availability
- Access safe & UH-verified running routes
- Log runs and track progress
- View route difficulty scores (heat, slope, humidity, distance)
- Share safety feedback (lighting, crowds, sidewalks, water fountains)

This creates a **motivating and safety-focused running community** built specifically for UH students.

This is also deployed to [Vercel](https://run-and-route-hub.vercel.app/).


Also check it out in our [Github Repository](https://github.com/orgs/run-and-route-hub)!

# My Contributions to the Project

Throughout the project, the team consistently communicated with each other, with multiple check ins and meetings. Here are some of my contributions to the team 

### 1. Sign-in and Sign-up Pages

In this project I was in charge of developing the authentication pages, which allowed users to register, log in, and access their protected data securely using any emaill they have in our system. Users are able to log in/log out successfully, and protected pages redirect unauthenticated users. 

### 2. Set up database schema 

In the project I was in charge of the website functional design, and implemented my ideas through the database schema I pushed. Using Prisma, I defined model for users and routes, and tested the schema with seed data as shown below. 

```prisma
model User {
  id                  Int               @id @default(autoincrement())
  email               String            @unique
  password            String
  role                Role              @default(USER)
  displayName         String?
  location            String?
  paceMin             Float?
  paceMax             Float?
  preferredDistanceKm Float?
  terrainPreference   TerrainPreference?
  experienceLevel     ExperienceLevel?  @default(BEGINNER)
  bio                 String?
  daysAvailable       String[]          @default([])
  prefersMorning      Boolean           @default(false)
  prefersAfternoon    Boolean           @default(false)
  prefersEvening      Boolean           @default(false)
}

model Route {
  id           Int        @id @default(autoincrement())
  name         String
  distanceKm   Float
  distanceMile Float
  colorr       Int
  colorg       Int
  colorb       Int
  path         Location[]
}
```

### 3. Implementing User Profile

Utilizing my implemented database schema, I was able to generate a mock up user profile page that shows User ID, location, date signed up, along with "stat snapshots" of last 30 days of running

I separated the task into two different components, a ProfileHeader.tsx, and a StatsOverview.tsx. This allowed my group to have a realistic UI demonstration on how the user profile would appear for the application

### 4. Implementing Route Review Function

As our project finalizes, I implemented a user route review system that allows the user to search, choose, and rate/review routes based on their enjoyability and difficulty. 

# User Guide

## Landing Page
<img src="images/M2/M2LandingPage.png">
This is our landing page, featuring our purpose in the center with multiple text blocks beneath it going into detail about the different features we have.

## About
<img src="images/M2/M2About.png">
For a more in depth dive into the intentions, goals, and purpose of this project.

## Routes
<img src ="images/M2/M2Routes.png">
This page shows some off some of the routes on a map with there start and end points labelled.

### After the User is Signed in

## Add Run
<img src ="images/M2/M2AddRun.png">
This page allows you to use a google map to choose the start and end points for your run. Once you select your route and give it a name it will show up in the routes page.

## Find Run
<img src ="images/M2/M2FindRun.png">
This page will allow you to search for runs based on certain criteria allowing you to find routes personalized to your search.

## Find Running Buddies
<img src ="images/M2/M2RunningBuddies.png">
This page will allow you to find other runners and interact with them whether it is allowing you to schedule runs with them or just talk.

### Profile
<img src="images/M2/M2Profile.png">
This page can be found under the email where you will have stats associated with your account making it easier for you to be found by other users.

### Review Page

<img src="images/M3/Review.png">
This page is the other end of the find running buddies that allows you to view all the routes and click on one you wish to review. An option to search using ID is available in the search bar.

<img src="images/M3/Review2.png">
Clicking on a route allows you to rate the difficulty, enjoyability, and give additional feedback. 

# My take away 

Working on UH Run and Hub and with my incredible teammates opened my mind to a new understanding of software engineering beyond programming. I learned about design patterns, Github Issue managment using mile stones, ESLint rules, and even thorough communication with my team.

I was able to learn about effective communications, effort estimation and project timeline thanks to the teammates that I got to know and work with through this project. I gained confidence in presentation, coding review, and front end programming. Working closely with UI components enhanced my experience and ability to crtically think (what would my user want?) about the needs of the program and how it can be translated to a working UI. 