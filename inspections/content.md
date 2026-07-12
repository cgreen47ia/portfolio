---
title: Mobile Inspections App
category: Facilities
badge: accent
badge_label: Facilities
description: A field inspection tool for creating and capturing checklists and notes during property or quality reviews.
meta_description: Mobile Inspections App — a field inspection tool for creating and capturing checklists and notes during property or quality reviews.
year: 2026
role: Designer & Developer
tools:
  - HTML
  - CSS
  - React
  - Figma Make
  - Cursor
  - Netlify
  - Figjam
live_url: https://benevolent-taiyaki-8ec17b.netlify.app/
github_url:
---

## Overview

This mobile web application allows field workers on a construction site or at a warehouse facility to inspect materials and items on a regular basis from their mobile phone. Users can find inspections, view the details of them, execute an inspection and create a new inspection from this application. There is also a light and dark theme provided.

## Problem

Inspections are an every day necessity at construction jobsites and warehouses. A lot of machinery sits in one location, waiting to be used for months to years. However, they need to ensure the machinery stays in serviceable condition over this period of time. Inspections help with this process. By having a quick and easy way of creating, viewing, and executing inspections from a mobile device, field workers have a more convenient way of managing these inspections.

## Process

3 User Tasks > 3 User Flows > Site Map > Descriptives > Figma Make Prototype > Iterations in Cursor > Deploy to Netlify

I first identifed 3 tasks that users need to conduct: complete (or execute) an inspection, create a new checklist, and update an inspection checklist item. From here, I created 3 users flows (1 for each task) that demonstrates the actions users need to take and the screens they need access in order to complete the task successfully.

From here, I created a site map for this application which supports all user flows and then created a semantic version of all user flows and the site map that AI can best parse and use. Then I used these semantic flows and site map to construct the initial prompts and then create the application using Figma Make. I then continued to prompt Figma Make until the first user flow was created.

I then exported the code from Figma Make and imported into Cursor. Once I got the application up and running in Cursor, I prompted until the last two user flows were available in the application.

I also created a light theme and dark theme for this application. Users can toggle between each theme through a toggle button in the navigation bar. Once the application was completed, I deployed it to Netlify.

## Solution

This mobile application allows users to view all available inspections, search for and find specific inspections, create new inspections.

## Designs

### Home dashboard

On the home page, users can view their most urgent inspections that need their attention first. In addition, they can also view some quick KPIs about their inspections, such as how many have been completed and are in progress. Users can also view their to-do list for the day.

### Inspections list

When users navigate to Inspections, they can view all inspections and search and filter to find inspections. They can also read due dates and statuses of these inspections.

### Create inspection

When users click the Create Inspection button, they are taken to this screen, where they can choose a name for their inspection, create checklist items for the inspection and they can also launch into a preview.

### Inspection preview

When users launch into a preview of an inspection, they can view it from the inspector's eyes. What will the inspector see on the screen when they execute an inspection? This gives the user the ability to then make corrections or changes prior to creating or updating an inspection.


## Reflections

Right out of the box, Figma Make produces a nicer looking user intuitive compared to Cursor. This assumes no design system is created and used in advance. It's initial versions of the application were designed quite nicely, although it also made some strange decisions intially as well.

I also learned how to export code from Figma Make to use it in other systems, such as Cursor.
