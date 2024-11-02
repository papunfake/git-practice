# Git Guide

## 1. Setting Up Git

### 1.1 Installing Git
- **Windows**: Download and install Git from [git-scm.com](https://git-scm.com).
- **Linux (Ubuntu)**:
  - sudo apt update
  - sudo apt install git

- **Verify Installation**:
  - git --version
  *(This should display the Git version installed.)*

### 1.2 Configure Git (One-Time Setup)
Set up your username and email to track who makes changes:
- git config --global user.name "Your Name"
- git config --global user.email "your_email@example.com"

To view your configuration:
- git config --list

## 2. Starting with Git Basics

### 2.1 Initializing a Git Repository
Navigate to the folder where you want to track files:
- cd /path/to/your/project
- git init
*(This creates a `.git` folder, which tracks your project’s changes.)*

### 2.2 Adding Files to Staging Area
- Add a single file to the staging area (prepares it for commit):
  - git add filename.txt
- Add all files in the folder:
  - git add .
- Remove a file from staging (remove track permission):
  - git rm --cached filename.txt

### 2.3 Committing Changes
After staging, commit to save a snapshot of your project:
- git commit -m "Your commit message"

**Example**:
- git commit -m "Initial commit with main files"

### 2.4 Checking Repository Status
View the current status of your repo:
- git status

### 2.5 Viewing Commit History
Check the history of commits:
- git log

### 2.6 Restore Deleted File
To restore a committed file:
- git restore filename.txt
