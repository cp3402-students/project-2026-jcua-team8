# project-2026-jcua-team8
project-2026-jcua-team8 created by GitHub Classroom
## Purpose

This project involved the design, development, deployment, and documentation of a professional WordPress website for a real client, Kalynda Chase Tennis Blast. The goal was to improve the organisation’s outdated website by enhancing user experience, streamlining the booking process, and effectively showcasing coaching services and staff expertise.

This repository contains our team’s custom WordPress theme along with all supporting project documentation. It provides a complete record of our development progress and version control. The repository supports collaboration by tracking individual contributions, commits, and project progress through GitHub.

Our development process involved setting up multiple environments. We initially attempted to use Docker for local development to simulate a real-world workflow; however, due to configuration challenges, we transitioned to a different approach using AWS Lightsail for staging and deployment and developing on another local tool called LocalWP which we used in CP3402 subject practicals. This allowed us to work on the website locally and then host a live version of the WordPress site and enabled team members to access project files, changes and improve the website.

For team communication and collaboration, we first connected through Slack as required, and later adopted Discord as our primary communication platform due to its ease of use and real-time coordination features. This supported effective teamwork, task allocation, and problem-solving throughout the project.

The repository also acts as a professional, let's call it, "handover package", documenting how to install, develop, test, and deploy the website across local and cloud environments. This ensures that another developer can continue the project without ambiguity and major problems. Additionally, it provides transparency for markers by clearly demonstrating our workflow, project versions, and overall development process.

## Core Requirements

Our team delivered the following:

* A custom WordPress theme built from a recognised starter theme, customised to meet the client’s needs
* Local development using LocalWP, alongside a functional cloud-based staging and production environment using AWS Lightsail
* A public GitHub repository to manage version control and collaboration
* A project management board (Trello) to track tasks, responsibilities, and progress
* Comprehensive Markdown documentation outlining setup, workflow, and deployment processes
* A recorded workflow presentation demonstrating our development approach, tools, and team collaboration

This project demonstrates both the final product and the professional development practices used to achieve it, including teamwork, communication, version control, and deployment strategies.


## Documentation

All project documentation is written in Markdown and located in the `/Documentation` folder.

- [Deployment Guide](Documentation/deployment.md)  
  Explains how to set up the local environment, manage changes, test, and deploy the site.

- [Theme Documentation](Documentation/theme.md)  
  Describes the custom theme structure, features, and development decisions.

- [Site Management Guide](Documentation/site.md)  
  Explains how to manage content, pages, and plugins within WordPress.


## Project Links

- **Production Site (Live):**  
  todo link here

- **Staging Site (Development):**  
  todo link here

- **GitHub Repository:**  
  https://github.com/cp3402-students/project-2026-jcua-team8


## Repository Structure (Important Files)
major-staging-versions/
├── v1/
├── v2/
├── v3/
├── v4/
└── ...                # Each folder = snapshot of a major staging version

major-production-version/
└── final/             # Final production-ready version of the website

Documentation/
├── deployment.md      # Setup and deployment workflow
├── theme.md           # Theme structure and design decisions
└── site.md            # WordPress content management guide

wp-content/
└── themes/
    └── picostrap-child/   # Active custom theme (main development work)
