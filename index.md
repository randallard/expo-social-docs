---
layout: home
title: Home
nav_order: 1
permalink: /
---

# Expo Social App Documentation

Welcome to the documentation for the Expo Social app, a tool for playing with friends.

## What is the Expo Social?

Expo Social is a way to play games and connect with your friends.

## About This Project

This app allows users to:
- Play Expo Social games with friends
- Earn points and acheivements

## Project Status
{: .fs-5 }

Want to know where we are in development? Check our [Project Plan & Status]({{ '/docs/project-plan-and-status' | relative_url }}) page to see our current progress, upcoming milestones, and development roadmap.

[View Project Status]({{ '/docs/project-plan-and-status' | relative_url }}){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

## Latest Development Update
{: .fs-5 }

{% assign latest_entry = site.html_pages | where: "parent", "Development Journal" | sort: "date" | reverse | first %}
{% if latest_entry %}
### [{{ latest_entry.title }}]({{ latest_entry.url | relative_url }})
**Date:** {{ latest_entry.date | date: "%B %d, %Y" }}

{{ latest_entry.excerpt | truncate: 150 }}

[View latest update]({{ latest_entry.url | relative_url }}){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[Development Journal]({{ '/docs/development-journal' | relative_url }}){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }
{% else %}
Development journal entries coming soon!

[Development Journal]({{ '/docs/development-journal' | relative_url }}){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }
{% endif %}

## Getting Started

To begin using or developing the app, check out the [Getting Started]({{ 'docs/getting-started' | relative_url }}) guide.