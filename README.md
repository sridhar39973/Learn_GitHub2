## To push new folder from vs code to github
#Step 1:
Create a folder and open it in VS Code:

Create a new folder on your local machine.
Open the folder in Visual Studio Code.
Add a dummy file in that folder:
# Step 2:
Inside the folder, create a new file (e.g., dummy.txt).
Initialize an empty Git repository:
# Step 3:
git init
Check the status of the Git repository:
# Step 4:
git status
The dummy.txt file will be in an untracked status.
# Step 5:
Add the dummy file to the staging area:
git add .
#  Step 6:
Check the status again:
git status
The dummy.txt file will now be in the staged status, ready for committing.
# Step 7:
Commit the staged file:
git commit -m "Initial commit with dummy file"
# Step 8:
Create a new repository on GitHub:
Go to your GitHub account.
Click on the "New" button to create a new repository.
Name your repository and do not initialize it with a README, .gitignore, or license (since you've already initialized a repository locally).
# Step 9:
Add the remote origin to your local Git repository:
git remote add origin <copied GitHub HTTPS URL>
# Step 10:
Check the current branch:
git branch
By default, this will likely show the master branch. If you want to rename it to main (or vice versa), you can use the next step.
# Step 11:
Rename the branch if needed:
git branch -M main  # If you want to rename 'master' to 'main'
# or
git branch -M master  # If you want to rename 'main' to 'master'
Push the file to the remote repository:

git push origin main  # or 'git push origin master' depending on your branch name
