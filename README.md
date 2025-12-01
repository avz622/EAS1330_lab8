# This is a title
## This is a subtitle
*This text is italicized*
**This text is bold**

# EAS 1330 Lab 8



This document will show a summary of the steps performed during Lab 8. 



## 1. How the Repository Was Created



The remote repository was created on GitHub:

1.  Logged into GitHub and navigated to New Repository.

2.  Named it `EAS1330_Lab8`.

3.  I made sure that I did not start it with a README so that I could practice adding files later via the command line.

4.  The initial `README.md` was created and committed on the GitHub website before cloning.



## 2. Git Configuration and SSH Setup



Before connecting to GitHub from the Linux environment, I performed the following configuration steps:



### A. Identify Git

This makes my commits with my identity.

```bash

git config --global user.name "Your Name"

git config --global user.email "your_github_email@example.com"



## 3. The Core Git Workflow (Clone, Commit, Push, Pull)

### The Clone Operation
I copied the remote repository to my local Linux environment  using the SSH URL. This creates a local copy that tracks the remote history:
```bash
git clone git@github.com:username/EAS1330_Lab8.git

git add .:Made local changes
git commit -m "A message describing the update": Created a local snapshot of the changes with a descriptive message.
git push: Uploaded the committed history to GitHub.
git pull: To get updates made by others to my local copy, I used:

## 4. How to Fix Sync Issues: 



If the local repository becomes corrupted, the safest way to fix it is to delete the local directory and re-clone the clean, guaranteed-safe version from GitHub.



1.  Go up one directory: `cd ..`

2.  Delete the local copy: `rm -rf EAS1330_Lab8`

3.  Re-clone the clean copy: `git clone git@github.com:username/EAS1330_Lab8.git`

This is safe because the complete version history remains backed up on the GitHub server.
