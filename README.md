# GitHub Collaboration Guide

This guide explains how to collaborate on a project using GitHub. Follow these instructions to set up and manage group projects.

## Table of Contents
1. Initializing a New Project
2. Setting Up Your Team
3. Collaborating with Branches
4. Submitting a Pull Request
5. Merging a Pull Request

   ## Initializing a New Project

   **Create a Local Repository**:
   - Open IntelliJ and create a new project.
   - Click the `Terminal` icon on the bottom left. Click the `New Predefined Session` dropdown and choose `Git Bash`.
   - Create a local git repository by entering git init.
   - ``` bash
      git init
      ```
   **Create a New GitHub Repository**:
   - Go to GitHub, click the `+` button, and select **New Repository**.
   - Enter the repository name and description.
   - Select public or private visibility based on your team’s needs.
   - Do **not** initialize with a `README.md`. You will create that manually later.
   - Click **Create Repository**.
  
   **Link Your Local Repository to GitHub**:
   - Copy the repository URL from GitHub.
   - In your Git Bash, run:
     ```bash
     git remote add origin <repository-url>
     git branch -M main
     git push -u origin main
     ```
     *Found on GitHub project home page*

     Your Git Bash should look like this when you’re done:

     ![result of linked repo](screenshots/resultOfGithubRepo.png)

   This adds a ‘.git’ folder to your repo, connects you to your remote Github Repo and also gives you a ‘.gitignore’ file.
   
   ![git ignore added](screenshots/gitIgnoreImage.png)

   And if you go to your Github Repo page and refresh, you’ll see the ReadMe that you intialized with and the reference to the first commit you made.

## Set up your team
Click on the "Settings" tap of your rep, then "Collaborators" then search for GitHub users and add them by clicking "Add Collaborators":
<img width="1314" alt="Screenshot 2024-09-17 at 3 40 36 PM" src="https://github.com/user-attachments/assets/0fd27492-e3a6-4b0a-b378-123b1fa1663f">

They will receive an email letting them know you added them and will be listed as a collaborator:
<img width="675" alt="Screenshot 2024-09-17 at 4 00 42 PM" src="https://github.com/user-attachments/assets/6da93ccb-d975-4737-bee9-77c1e0f653f1">


Your team worked hard on their features in separate branches and now it's time to merge them into the Master branch for deployment. Establishing a Git Flow is crucial for teamwork.

Assign one person to manage merging, like a "Reviewer" or "Merge Master," to avoid conflicts.
Everyone should git push their branches for review and merging.

<img width="684" alt="Screenshot 2024-09-17 at 4 42 41 PM" src="https://github.com/user-attachments/assets/2c773a73-5ebe-4e41-a889-085661069913">

Now, navigate to the GitHub repository page. You should see the branch you pushed in a yellow bar at the top with a "Compare & pull request" button.

<img width="658" alt="Screenshot 2024-09-17 at 4 43 47 PM" src="https://github.com/user-attachments/assets/0ca7fdc1-fb48-47ee-96cc-07a20863c009">

Click "Compare & pull request," which will take you to the "Open a pull request" page. Write a brief description of the changes you made. Then, under the "Reviewers" tab, select your team's "Merge Master." Finally, click "Create pull request."

<img width="675" alt="Screenshot 2024-09-17 at 4 45 23 PM" src="https://github.com/user-attachments/assets/6533063a-5034-4ebf-a4c2-bf29597db1ad">
