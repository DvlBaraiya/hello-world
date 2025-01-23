This repository is for practicing the GitHub Flow.

## Initial Setup

1. Open the command prompt and navigate to the directory where you store your code.
   ```bash
   cd /path/to/your/code
   ```
2. Initialize Git:
   ```bash
   git init
   ```
3. Clone the repository:
  ```bash
  git clone https://github.com/ChaitanyaGCB/VerizonTracker.git
  ```
4. Navigate to the project directory:
  ```bash
  cd VerizonTracker
  ```
5. Create a new branch (replace "your_name" with your actual name):
  ```bash
   git checkout -b "your_name"
   ```
6. Push the branch to the remote repository: (replace "branch_name" with your actual branch name)
  ```bash
  git push -u origin "branch_name"
  ```

## Regularly Sync with main
Make sure you are using latest main branch before you start coding.
1. Make sure you are inside Your Branch:
   ```bash
      git checkout "branch-name"
   ```
3. Pull the latest Main Branch
   ```bash
   git pull origin main
   ```
4. Resolve Any Merge Conflicts (if applicable):
If there are merge conflicts, Git will indicate them. Resolve the conflicts in your editor, then stage and commit the resolved files:
   ```bash
   git add .
   git commit -m "Resolved merge conflicts with main"
   git push
   ```


## JIRA Integration Workflow
1. Start a Task:
  Move the JIRA task from "To Do" to "In Progress".
2. Commit Changes
  Commit code based on tasks mentioned on JIRA.
  Try to commit code in github at least once for each task on JIRA.
  ```bash
    git add .
    git commit -m "JIRA Task description / additional comments"
  ```
3. Complete the Task:
  Move the task in JIRA from "In Progress" to "Done"
4. Push Changes
  Push the code to the GITHUB after each commit or once done with all tasks (whichever you prefer)
  ```bash
    git push
  ```
## Branching Guidelines
Always use your branch for commits.
Do not commit or push or merge directly into the main branch unless explicitly instructed.

## Merging Branch into main (Only if instructed)
Follow these steps to merge your branch into the main branch:

1. Switch to the main Branch: Make sure your local main branch is up-to-date:
   ```bash
     git checkout main
   
     git pull origin main
   ```
2. Merge Your Branch into main: Merge your branch (replace "branch_name" with your branch name) into main:
   ```bash
     git merge "branch_name"
   ```
3. Resolve Conflicts (if any): If there are merge conflicts, Git will notify you. Open the conflicting files, resolve the issues, and then add the resolved files:
  ```bash
    git add .
    git commit -m "Resolved merge conflicts"
  ```
4. Push the Updated main Branch to Remote: Once the merge is complete, push the changes to the remote repository:
   ```bash
     git push origin main
   ```

