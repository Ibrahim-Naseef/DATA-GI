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

- clone : used to download repo from github to local machine
  `git clone <link>

- status : displays staus of code or file

1. untracked : new files which are not added
2. modified : file that content are changed
3. staged : file is ready to be commited
4. unmodified : didnt change any content of file

- add : To add the modified file to staged state
  `git add <file>`

- commit : Keeps records of all changes
  `git commit -m <message>`

- push : Upload local repo to remote repo
  `git push origin main`
