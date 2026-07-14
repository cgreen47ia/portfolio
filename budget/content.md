---
title: Monthly Budget Web App
category: Finance
badge: warning
badge_label: Finance
description: A personal finance tracker for monitoring spending, setting category limits, and staying on top of monthly goals.
meta_description: Monthly Budget Web App — a personal finance tracker for monitoring spending, setting category limits, and staying on top of monthly goals.
year: 2026
role: Designer & Developer
tools:
  - HTML
  - CSS
  - React
  - Cursor
  - Netlify
  - Figjam
live_url: https://courageous-malasada-41727c.netlify.app/
github_url:
---

## Overview

Monthly Budget Web App is a personal finance tracker built to make everyday money management feel clear instead of overwhelming. Users can categorize spending, set monthly limits by category, and see at a glance whether they are on track against their goals.

Built with the Veridian Compass design system inspired by Nerd Wallet's website design, the interface uses strong typographic hierarchy and high-contrast color fields so financial data stays readable and actionable — whether checking a quick balance or reviewing spending patterns at the end of the month.

## Problem

Most people know they should track spending, but spreadsheets and complex finance apps create friction. Without a simple view of where money goes each month, it is easy to overspend in small categories and lose sight of larger financial goals. Users need a lightweight tool that surfaces the essentials without requiring accounting expertise.

## Process

3 User Tasks > User Flows > Site Map > Design System > Iterations in Cursor > Deploy to Netlify

From an app idea, I created 3 distinct user tasks that users would need to conduct: entering a monthly income, adding expenses to a category, and adjusting category limits when overspending occurs. From these tasks, I created detailed user flows, detailing user actions, system actions, and screens to support each task.

I then created a site map, showing the pages, their sections, and how the pages are related. From here, I converted these user flows and site map into a descriptive version in markdown format that AI can parse and understand.

I then created a skill in Cursor that can convert any existing website into a design system. The skill does not include proprietary designs from these web pages. I used this skill to convert Nerd Wallet's web design into a design system, which resulted in the creation of a DESIGN.md file. This file served as the styling and design system source of truth for this application.

From here, using the user flow markdown versions, I prompted Cursor to create the application one step at a time, by creating site pages and user flows. I then iterated on the designs by ensuring the user flows worked without bugs and by making changes to the output. Once complete, I deployed the application to Netlify.

## Solution

The app centers on a monthly dashboard that shows category breakdowns and spending in one view. Users add transactions quickly, assign categories, and set per-category limits that update in real time. Visual progress indicators make it obvious when a category is approaching its cap or is overspent, encouraging smarter spending decisions before the month ends. Users can also move money from one category to another to account for overspending, which helps in months where spending needs are variable.

## Designs

### Upcoming expenses dashboard

The home view gives users a calm overview of their monthly budget — surfacing income, categories, and a chronological list of upcoming expenses so they can anticipate spending before it happens.

### Budget overview

The budget page combines monthly income entry with category cards that show spending totals and progress bars. Users can see how each category is tracking against its limit at a glance, with alerts when spending exceeds a cap.

### Edit expense

From any category, users can update or delete individual transactions through a focused edit modal. Overspent categories are flagged inline with visual progress indicators, making it clear when a limit needs attention.

### Category management

The categories view organizes every budget area in a scannable grid. Users can add expenses, edit category spending limits, and reallocate budget when a category goes over — keeping variable monthly needs under control.

## Reflections

This was the first AI-generated web application I created using this process. Overall, I was suprised at the efficiency of creating a multi-feature web app with the process, and the ability to create a consistently applied design system. Basing the prompts and designs on user flows and interaction patterns established a user-centered approach to this AI-aided web application. 

This project strengthened my process to designing and building web applications with AI. Future improvements to the app could include recurring transaction support, export to CSV, and month-over-month comparison views.