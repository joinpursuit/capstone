# Git and GitHub with Teams

### Git Refresher

So far, you have been using git to get code (pull) from a remote repository (on github), writing your own code, tracking it with git, and moving (push) the code from your computer (local version) to github.

When using git locally (on your computer), you have been running the commands in Terminal (Command line).

A git command has a minimum of 1 argument.

Git commands are always executed by first typing `git`

The first argument is the command (or verb), like

- `git init` (initialize a new git repository)
- `git push` (send the code to a remote location)

The second(+) argument gives the first argument context (when needed)

- `git add .` (add all files in this directory)
- `git pull origin master` (get all files from the url that has an alias of `origin`, from the branch `master`)

Lastly, flags can be added

- `git remote -v` (git show remote(s) and be verbose(give more detail))

Here is a table of our commonly used git commands that we've used in this course so far:

| git | Argument |                                    Flag(s)/Additional arguments                                     |                                                                  Description                                                                   |
| :-: | :------: | :-------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------: |
| git |   init   |                                                                                                     |                                                          Initializes a new repository                                                          |
| git |   add    | `.` (everything on this directory level and lower) or filename or `-A` (all the files in this repo) |                             Takes untracked files and adds them to the staging area so that they can be committed                              |
| git |  commit  |                                          -m 'some message'                                          |                             Takes a snapshot of files in the staging area/ saves this version of them as a commit                              |
| git |  remote  |                                                 -v                                                  | Shows the remote repositories associated with the local repository. Most repositories have an alias for their urls like `origin` or `upstream` |
| git |   pull   |                                           upstream master                                           |                                   Gets files from a url with an alias of `upstream` from its branch `master`                                   |
| git |   push   |                                             origin dev                                              |                                       Sends files to a url with an alias of `origin` to its branch `dev`                                       |
| git |   log    |                                              --oneline                                              |                              Shows a log of commits of a repo (--oneline shows a truncated message)_`q` to exit_                               |
| git |  status  |                                                                                                     |                                        Shows the state of files in a repo (untracked, modified, staged)                                        |
| git |   log    |                                              --oneline                                              |                                                          see a short list of commits                                                           |

[Link to our wiki with a more complete list of git commands](https://github.com/ga-students/wdi-remote-matrix/wiki/Git-Cheatsheet)

Note: `fork` is not on this list because `fork` is not a git command; it is github-specific for copying a repository on github to a new location on github.

### Git VCS - Branches and Merging

Git is a VCS (Version Control System). There are a few popular ones, but git ends up being a top choice because of its branching and merging feature.

If we think back to our past projects, when we wanted to implement some major changes to our code and failed our popular options were to

- `⌘Z` throughout our files and hope for the best
- Comment out a ton of code and hope to restore the functionality of our code to a previous version
- Seriously contemplate coding out our project from scratch again
- Curl up into a ball and hope the code would revert via magic

[Git's about page has 4 great reasons why it works so well for individuals and large teams.](https://git-scm.com/about)

- Frictionless Context Switching - Switch between branches, whenever! No worries!
- Role-Based Code Lines - Have many versions of your code - Production, Development, Day-to-Day etc.
- Feature Based Workflow - Create a new branch for each feature
- Disposable Experimentation - if a branch doesn't work out, you can just walk away or toss it. It has no impact on the working code

You may be thinking 'this sounds too good to be true!' It's not! But there is a catch! Git requires changing the way we are used to working on projects. Which means it takes some time and practice to learn to use git.

![git workflow from git about page](https://i.imgur.com/MXiZRI0.png)

(image from https://git.scm/about)

### New Git Commands

To be able to use branches, we will have to learn some new git commands

| git | Argument | Flag(s)/Additional arguments |                              Description                               |
| :-: | :------: | :--------------------------: | :--------------------------------------------------------------------: |
| git |  branch  |                              |                             Lists branches                             |
| git |  branch  |         branch_name          |                          Creates a new branch                          |
| git | checkout |         branch_name          |                           Switches branches                            |
| git | checkout |      -b new_branch_name      |            Creates a new branch and switches to that branch            |
| git |   diff   |                              |    Let's you see the changes that you have made (before `git add`)     |
| git |   log    |      --graph --oneline       | See a short summary of commits and branches (press q to exit the view) |

Even though these are just five new commands, it is going to take some practice to master them.

Note: You may have noticed that `git merge` is missing - we will be merging our branches via github, so we will not use this command today.
