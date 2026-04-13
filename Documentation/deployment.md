starting note: we were initially going to use docker for local development with a script linking github and lightsail server. Unfortunately, after a long time trying to set it up and get it to work, this did not work and we had to use another method. We contacted our mentor asking for help. We were told to use whatever method works for us and gets us going. Therefore, we used the local tool we used in the CP3402 practicals.

# Deployment Guide

This document explains the development and deployment workflow used in this project. It is written so that a new team member can follow the same process to continue development and safely deploy changes.

## Local Environment Setup

Local development is performed using LocalWP.

We initially attempted to use Docker and automate deployment between GitHub and the AWS Lightsail server. However, due to configuration issues and lack of server access, this approach was not viable. As a result, we adopted a simpler and more reliable workflow using LocalWP.

### Steps to set up locally:

1. Install LocalWP
2. Create a new WordPress site
3. Install the UpdraftPlus plugin
4. Import a backup of the current website using UpdraftPlus:
   - Database
   - Plugins
   - Themes
   - Uploads
   - Other files

This creates a fully working local copy of the website.

## Making and Committing Changes

All development changes are made locally using the WordPress admin interface in LocalWP.

### Workflow:

1. Make changes locally:
   - Edit pages, content, and settings via WordPress
   - Modify theme files if required

2. Backup changes using UpdraftPlus:
   - Create a full backup (database + files)

3. Commit to GitHub:
   - Commit the updated version into:
     ```
     major-staging-versions/
     ```
   - Each folder (e.g. v1, v2, v3) represents a major staging version

This repository is used to track major versions, not every minor change.

---

## Testing Changes

Testing is performed on the staging server (AWS Lightsail).

### Process:

1. Take the latest local backup
2. Upload it to the staging WordPress site
3. Restore using UpdraftPlus
4. Verify:
   - Pages load correctly
   - Navigation works
   - Buttons and links function
   - Layout matches local version
   - No visual or functional errors

All major changes must be tested on staging before being considered complete.

---

## Deployment to Staging

The staging server is hosted on AWS Lightsail (WordPress instance).

### Steps:

1. From LocalWP:
   - Create a full UpdraftPlus backup

2. On staging site:
   - Install UpdraftPlus (if not already installed)
   - Upload backup files
   - Restore the site

3. Test the deployed version thoroughly

The staging server acts as the main shared environment for the team.

---

## Deployment to Production

Production represents the final live version of the website.

Only fully tested and stable versions from staging are deployed to production.

### Process:

1. Confirm staging version is complete and working correctly
2. Deploy the same backup to the production site
3. Perform final checks:
   - Functionality
   - Layout
   - Links and navigation

4. Save this version in the repository under:
