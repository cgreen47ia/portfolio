---
title: Sweat Equity
category: Fitness
badge: cta
badge_label: Fitness
description: A mobile-first web application that encourages students to exercise by cashing in exercise points for mentorship opportunities.
meta_description: Sweat Equity — a mobile-first fitness app that rewards student exercise with mentorship opportunities.
year: 2026
role: Designer & Developer
tools:
  - HTML
  - CSS
  - React
  - Cursor
  - Supabase
  - Netlify
  - Figjam
live_url: https://sweat-equity.netlify.app/
github_url: https://github.com/cgreen47ia/Final-Project
---

## Overview

Sweat Equity is a mobile-first web application built for students who want to stay active and unlock real-world career opportunities. The app tracks exercise activity, converts effort into redeemable points, and lets users cash those points in for mentorship sessions with industry professionals.

## Problem

Many students struggle to maintain consistent exercise habits with a busy schedule, especially when motivation fades mid-semester. Traditional fitness apps focus on personal stats but rarely connect physical activity to meaningful career or academic growth. Students need a more motivating reason to exercise beyond the gym — something that ties effort to career opportunity. This problem and potential solution was uncovered during 6 1-hour user interviews with current college students.

## Process

4 User Tasks > User Flows > Site Map > Moodboard > Design System > Create & Iterate in Cursor > Database Setup > Iterate More > Testing > Deploy to Netlify

From an app idea, I defined 4 distinct user tasks: log workouts, view, favorite, and prioritize mentorship opportunities, view progress towards mentorships, and redeem points for a mentorship session. These tasks shaped the core motivation loop — activity, reward, opportunity — and became the foundation for detailed user flows covering user actions, system responses, and the screens needed at each step.

I then created a site map showing how the home, mentorship, and workout pages connect across mobile and desktop layouts. From there, I converted the user flows and site map into markdown descriptives that AI could parse and use as build context.

I then created multiple UI designs through sketching ideation, creating at least 5 design options per screen. I then evaluated the sketches and chose one winning sketch per screen.

Next, the application needed a design system. I created a moodboard to capture the look and feel I wanted the application to have. Next, I prompted cursor to create a design system based on this moodboard across multiple prompts, resulting in a DESIGN.md file. Both light and dark themes are reflected in this design system.

I then constructed a PLAN.md file which included prompts that would create the application structure, user flows, screen elements, design system, and database schema. I then executed this plan and the app was created. From there, many iterations were made to improve user flows, remove bugs, and improve consistency and user experience.

A Supabase database was then setup and connected to the application to store all necessary app data and to handle user accounts and authentication.


## Solution

Sweat Equity bridges fitness and mentorship by introducing an exercise-point economy. Students log workouts, earn points based on activity type and duration, and browse a catalog of mentorship sessions they can unlock. The mobile-first layout keeps tracking quick between classes, while the rewards screen makes progress tangible and aspirational. This solution encourages exercise by tying it to tangible career benefits, which was a problem discovered in past user interviews with college students.

## Designs

### Mentorship catalog

The mentorships view lets students browse available sessions, filter by topic and point cost, and see progress toward each opportunity. Cards surface mentor profiles, session descriptions, and point requirements so users can choose rewards that feel genuinely valuable.

### Mentorship detail

Each mentorship opens to a focused detail page with mentor bio, session objectives, and a progress bar showing how close the user is to unlocking the session. Favorite and delete actions keep the catalog personal and manageable.

### Workout selection

The new workout flow presents a grid of activity types — from yoga to HIIT to campus walks — each with a points-per-minute rate. Students can pair a wearable device and start a session with a single tap, keeping the highest-frequency action fast and thumb-friendly.

### Past workouts

The workouts history view lists past sessions with activity name, date, points earned, and duration at a glance. A prominent new workout button keeps logging fast, and the screen supports both light and dark themes for comfortable use any time of day.

### Workout complete

After finishing a session, users see time logged, points earned, and updated progress toward their active mentorship goal. The completion screen closes the motivation loop by connecting physical effort directly to the opportunity they are working toward.

## Reflections

Building Sweat Equity reinforced how gamification works best when rewards feel genuinely valuable — not just badges, but real mentorship access. Designing around a clear user-task loop made the mobile-first layout easier to prioritize, and the design system kept motivation high without letting the interface feel cluttered or game-like.

This project sharpened my skills in a robust user-centered design process while using AI applications like Cursor, as well as designing motivational flows that keep users coming back. Future improvements could include social challenges, recurring workout streaks, and integration with wearable device APIs for automatic activity tracking.
