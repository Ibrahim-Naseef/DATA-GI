# Git

**Git** is a version control system which is used to track changes made in a code or file.

- Track history
- Collaborators
- Fast and Secure

## Configuring Git

It is used to set username and mail so we can keep track that changes can be made from diffrent mail id.

- git config --global user.name "Name"
- git config --global user.mail "Mail@"
- git config list

## Git Commands

- **clone** : used to download repo from github to local machine
  `git clone <link>


- **status** : displays staus of code or file
  1. untracked : new files which are not added
  2. modified : file that content are changed
  3. staged : file is ready to be commited
  4. unmodified : didnt change any content of file


- **add** : To add the modified file to staged state
  `git add <file>`


- **commit** : Keeps records of all changes
  `git commit -m <message>`


- **push** : Upload local repo to remote repo
  `git push origin main`

## To create new Repo in Local and Upload it to Remote Repo

1. Create a new Repo. `mkdir NewRepo`
2. Change directory to that new Repo. `cd Newrepo`
3. Run `git init` command to initialize it as an Git Repository
4. Add files that are required.
5. Make a new repo in github
6. Run `git remote add origin <-git repo link->` to add to remote system.
7. Run `git remote -v` to confirm the path
