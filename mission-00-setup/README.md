# Mission 0 — Create your GitHub workspace

## 1. Task / objective


## 2. Work completed
- Repository name: the-digital-detective-8553

- Folders created: mission-00-setup mission-01-computer-basics mission-02-terminal mission-03-operating-system mission-04-programs mission-05-numbers-data mission-06-git-github mission-07-networking mission-08-final-report evidence

- Files created: 

## 3. Commands / tools used
- python3 --version: (purpose) , result: (your version)
- git --version: (purpose) , result: (your version)
- mkdir: (what it did for you)
- touch: (what it did for you)
- git init / add / commit / remote / push: (one line each on what it did)
- VS Code and Terminal: (how you used them)

## 4. My understanding
- What is a repository? 
A repository is a project folder that Git keeps track of. It holds your files plus a complete history of every change you’ve made to them.
- Why is the structure organised by mission? 

The folders are organised by mission so that each mission's work, notes and
README stay separate. This also makes the commit history easy to follow, because
each mission gets its own commit, and it makes my work easier for my instructor
to review.


## 5. Difficulties faced
1.When I ran touch README.md mission-0*/README.md, zsh showed
   "no matches found: mission-0*/README.md" and no README files were created.
2. My project folder was named the-digital-detective-8553, but the assignment's
   naming rule gives digital-detective-8553.


## 6. How I resolved them
1. I learned that zsh expands the * wildcard before running the command, and it
   only matches files that already exist. Since no README files existed yet,
   it failed. I fixed it by creating the root README separately and using a loop,
   for dir in mission-0*; do touch "$dir/README.md"; done, which matches the
   folders that already existed.
2. I renamed the folder so that it matches the GitHub repository name exactly.

## 7. Evidence / files
- mission-00-setup/README.md (this file)
- README.md (root README with the mission index)
- Folder structure created: 9 mission folders and evidence/

## 8. Commit details
- Commit message: Set up Digital Detective mission structure
- Pushed to GitHub:Yes, and I confirmed the commit and folders are visible
  on GitHub. 

 