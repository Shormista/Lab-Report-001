# Lab Report 001 - Version Control with Git and GitHub

## Project Description
This project demonstrates the complete Git and GitHub workflow for version control and collaboration.

## Files Included
- `shormi01.html` - Main HTML file with student admission form
- `shormi02.css` - CSS styling for the HTML page

## Git Workflow Demonstrated
- Repository initialization
- Adding and committing files
- Branching (main and feature-form)
- Merge conflict creation and resolution
- Pushing to GitHub

## Branches
- **main** - Contains Department field
- **feature-form** - Contains Student ID field

## How to Run
1. Open `shormi01.html` in a browser
2. The form includes both Department and Student ID fields

## Git Commands Used
```bash
git init
git add shormi01.html shormi02.css
git commit -m "Added shormi01.html and shormi02.css files"
git remote add origin https://github.com/Shormista/Lab-Report-001.git
git branch -M main
git push -u origin main
git checkout -b feature-form
git add shormi01.html
git commit -m "Added Student ID field to admission form"
git push -u origin feature-form
git checkout main
git add shormi01.html
git commit -m "Added Department field to admission form on main"
git merge feature-form
# Resolved conflict
git add shormi01.html
git commit -m "Resolved merge conflict: Combined Department and Student ID fields"
git push origin main
