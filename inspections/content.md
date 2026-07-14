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

I first identifed 3 tasks that users need to conduct: complete (or execute) an inspection, create a new inspection, and update an inspection checklist item. From here, I created 3 users flows (1 for each task) that demonstrates the actions users need to take and the screens they need to access in order to complete the task successfully.

From here, I created a site map for this application which supports all user flows and then created a markdown version of all user flows and the site map. This markdown version provides a format that AI tools can better understand and process. Then I used these markdown user flows and site map to construct the initial prompts and then create the application using Figma Make. I then continued to prompt Figma Make until the first user flow was created.

After the first user flow was created, I then exported the code from Figma Make and imported it into Cursor. Once I got the application up and running in Cursor, I used the markdown user flows to create  the last two user flows in the application. While the base flows worked in the application at this point, there were several inconsistencies with screen layouts and design elements. More iterations were required to create a higher level of consistency across all screens.

I also created a light theme and dark theme for this application. Users can toggle between each theme through a toggle button in the navigation bar. Once the application was completed, I deployed it to Netlify.

## Solution

This mobile application allows users to view all available inspections, search for and find specific inspections, create new inspections, and update existing inspections.

## Designs

### Home dashboard

On the home page, users can view their most urgent inspections that need their attention first. In addition, they can also view some quick KPIs about their inspections, such as how many have been completed and are in progress. Users can also view their to-do list for the day.

### Inspections list

When users navigate to Inspections, they can view all inspections and search and filter to find specific inspections. They can also read due dates and statuses of these inspections.

### Create inspection

When users click the Create Inspection button, they are taken to this screen, where they can choose a name for their inspection, create checklist items for the inspection and they can also launch into a preview.

### Inspection preview

When users launch into a preview of an inspection, they can view it from the inspector's eyes. What will the inspector see on the screen when they execute an inspection? This gives the user the ability to then make corrections or changes prior to creating or updating an inspection.

## Reflections

Right out of the box, Figma Make produces a nicer and more modern-looking user interface compared to Cursor. This assumes no design system is created and used in advance. At first glance, this initial version of the application was designed quite well, although Figma Make also made some strange design decisions and it lacked consistency between design elements. This led to more rework of the screens compared to projects that created a design system first before producing screens.

While this application reflects a simple version of an inspections mobile application, it is suprising just how much functionality can be created in a short time using AI-aided design and coding methods. Future design directions for this project could include the creation of inspection templates, more complex inspection and checklist types, and the addition of photos and images in inspections.
