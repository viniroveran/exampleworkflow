# Step 0: Cloning the repository // Done just once
- Open Git Bash on repositories folder

```
git clone https://github.com/viniroveran/exampleworkflow.git
cd exampleworkflow
```
From here on, this is how every user story is started.  
If you were not on main branch, first finish your work, open a merge request and execute the following commands after your merge request is approved:  
```
git checkout main
git pull
```
**Pull** downloads all the latest commits from the repository.

# Step 1: Starting a new user story
- Open Git Bash on repository folder
- Create a new branch

```
git checkout -b new-user-story
```

# Step 2: Working on a file
- Add a new file to the repository, called newfile.txt and write your name in it
- Add the changed file to your next commit
	git add newfile.txt

- Commit your changes
	git commit -m "Finish new user story"

# Step 3: Push local changes to remote
```
git push origin new-user-story
```
**Push** uploads all local changes to the repository.

### Steps 2 and 3 are repeated for every task in your user story

# Step 4: Opening Merge Request
- Go to GitHub Repository page and click on Pull requests
- Open Pull request

# Step 5: Wait for the rest of the group to approve your changes.
- After Merge Request is approved, go back to master and update your repository.
- Open Git Bash again and execute:
```
git checkout main
git pull
```

# Tips and Tricks:
- **Always** finish your work before checking out to another branch.
- Adding **all changed files** to commit:
	`git add .`
- Adding all files from a folder to commit:
	`git add Assets/Scripts/*`
- Removing a file from commit but not changing it's content:
    `git restore --staged Path/To/File`
- Restoring all changes on a file since last commit:
    `git restore Path/To/File`
- Changing branch (without creating a new one):
    `git checkout branch-name`
