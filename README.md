# Test repository for the course in Digital Technologies in humanities 2024. 
This is a repository you can use to try to get familiar with cloning from GitHub. 

Here's some good commands to know, if you end up working with Git and GitHub in the future: 

## Terminal Cheat Sheet

[Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

## Navigating Files and Directories

### Some Good Commands:

- `pwd`
  - Print working directory. See the name/path of the current working directory.
  
- `ls`
  - See the contents of our directory. It prints the names of the files and directories in the current directory.

- `ls –F`
  - Classify the output by adding a marker to file and directory names to indicate what they are:
    - `/` indicates a directory.
    - `@` indicates a link.
    - `*` indicates an executable.

- `clear`
  - Clears the terminal.
  
- `man ls`
  - Read its manual.
  - Press `Q` to exit.
  - To search for a character or word in the man pages, use `/` followed by the search term.

- `cd`
  - Returns to the home directory.

- `cd Desktop/shell-lesson-data/exercise-data`
  - Change directory from the home directory to another folder.

- `cd ..`
  - Move one step up the directory level.

- `cd -`
  - Go back to your last directory.

- `mkdir`
  - Make directory. Creates a folder (e.g., `mkdir thesis` creates a folder called thesis).

- `touch something.txt`
  - Creates a text file called "something" in the current directory.

- `rm something.txt`
  - Removes a file.

## Possible Workflow:

```bash
$ mkdir spaceships
$ git status
$ git add spaceships
$ git status
$ touch spaceships/apollo-11 spaceships/sputnik-1
$ git status
$ git add spaceships
$ git status
$ git commit -m "Add some initial thoughts on spaceships"
```

# Key Git Commands:

- `git status` shows the status of a repository.
- Files can be in:
  - Working directory (user view)
  - Staging area (preparing for commit)
  - Local repository (where commits are stored)
- `git add` moves files to the staging area.
- `git commit` saves the staged content as a new commit in the local repository.
- Write a clear commit message that describes your changes.

## Shortcut:

- Press `Tab` for auto-completion of directory names.

## Cloning a Remote GitHub Repository:

This process gets a local copy of the repository from GitHub.

1. Ensure you are in the correct directory.
2. Run: `$ git clone <url-to-repository>`

## Connect Local Folder to Remote GitHub Repository:

1. Create a new repository on GitHub.
2. Open Git Bash.
3. Change the current directory to your local project.
4. Initialize the local directory as a Git repository: `$ git init`
5. Stage the files: `$ git add .`
6. Commit the files: `$ git commit -m "First commit"`
7. Copy the remote repository URL from GitHub.
8. Set the remote: `$ git remote add origin <remote-repository-URL>`
9. Verify the remote: `$ git remote -v`
10. Push to GitHub:
    - If using the master branch: `$ git push origin master`
    - If not:
        1. Rename local branch: `$ git branch -m <new_name>`
        2. Push with the new branch name: `$ git push origin -u <new_name>`
    - If errors appear due to a recently created remote repo, force push using: `$ git push origin -u -f <new_name>`

## Workflow for Saving Your Changes to GitHub (Version Control):

1. Make changes.
2. Stage the changes with `$ git add`.
3. Commit your changes with `$ git commit -m "Message"`.
4. Push your changes with `$ git push origin main`.

