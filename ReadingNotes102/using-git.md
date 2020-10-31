[Reading Notes Home](README.md)

# What is Git?

- Git is the version control for files, folders and projects. Git uses local operations so you can skip the need of having history fetched from a server. It also reduces the likelihood of losing data and will track changes made to any files or directories. Files are either in a commited state, modified state or staged.


## Using Git

To get started using Git, you can import an existing repository from GitHub through a series of commands in the terminal. The steps to this process are listed below, or check out the step by step instructions at 
[Git Tutorial](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/#5)

## Create Directory/Add Repository

1. Open terminal
2. Start by finding documents folder through *cd documents*
3. Continue usind *cd* and *ls* commands followed by folder names to see where you are and where you want to go to import a repository.
4. Add an existing repository URL from github by *git clone 'addurlhere'*
5. *OR* Create folder through *mkdir 'addnamehere'*
6. Check where you are through *pwd* or *ls*
7. Repeat steps 2-6 however many times necessary to complete creating directory/adding repository
8. Continue by *code .* to open VS Code and make any changes

## The ACP Process

1. navigate through directory to target project by *cd 'filename'*
2. example: find README.md and check status by *git status*
3. should show message in **red**, *modified: README.md* **IF** changes have been made and saved
4. **A=ADD** use command *git add .* to stage for commit 
5. again, run *git status* to view README.md in **green** , showing it as modified and ready for commit
6. **C=COMMIT** add note of changes made to modified README.md through *git commit -m "changesmade"*
7. **P=PUSH** use command *git push origin master*
8. *repeat step 2*
9. should show *"nothing to commit, working tree clean"*
10. go check github, changes should show
