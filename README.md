# Welcome to Digifan

## Table of Contents

- Separation of Concerns
- Front End
- Back End
- Git Commands

## Separation of Concerns

- digifan-front-end will house all of the front end browser code

- diigifan-back-end will house the API

---

## Front End

### /digifan-front-end

- The "node-modules"folder contains all the packages and dependencies installed with the command _npm init_ which was used to create the project (do not mess with this folder).

- The "public" folder contains all the public info and index.html, the contents in this folder should not be modified other than creating new .html files in order to create more pages

- The "src" folder contains various contets that will be discussed in the next section

- ".gitignore" tells the git repository which files will not be changed so they will be ignored

- "package-lock.json" describes the exact tree that was generated, such that subsequent installs are able to generate identical trees, regardless of intermediate dependency updates

- The "package.json" file is the heart of the node project and will be modified before publishment, it is used to install dependencies, run scripts, and identify the entry point to our package

- README.md is the file you are currently reading and it contains project information

---

### /src

- The first child of "src" is the components folder which will house all of the various React components

- "/media" houses all of the project media, including images, videos, and logos

- "App.css" contains all of the styling properties for the project

- "App.jsx" renders the main app (use components to add to it)

- "App.test.js" tests the app. It will not be used

- "database.sql" houses the database information that will be used when the app is deployed. During testing, you should create a database using these tutorials: [Creating a Node/Express/Postgres API](https://www.youtube.com/watch?v=_Mun4eOOf2Q&t=585s)

- "db.js" creates the pool object which makes database queries

- "index.css" is another stylesheet. It exists but I have 0 clue what it links to yet. I assume "index.html"

- "index.js" loads the front end "App" component of the website

- I assume "reportWebVitals.js" reports web vitals?

- I also assume that "setupTests.js" sets up tests but we probably won't use that

---

## Back End

- database.sql will house the database information that will be used when the app is deployed

- server.js houses the main server that takes requests

- /routers stores the various routers the app will use

- db.js creates the "pool" object which is used to access the database

---

## Git Commands

### Setting up a Repository

- Go into an empty file where you will create your repository and enter "git init"

---

### Adding remote origin

- git remote add origin https://github.com/mattjohnson2424/digifan.git

---

### Pulling from remote origin

- git pull origin

---

### Staging and Commiting to a local repository

- git add [file] (enter "." for all files)
- git commit -m " [descriptive commit message] "

---

### Git logs and checking out

- "git log" to see the log of commits on your branch

- "git checkout [first 7 digits of the commit hash seen under *git log*]" to revert back to a previous commit

---

### Branching

- "git branch" to see all branches
- "git branch [name]" to create a new branch
- "git switch [branch]" to switch to a branch
- "git merge [branch]" merges the specified branch with the branch you are currently on

---

### Pushing to the remote repository

1. Create a new branch
2. Switch to that new branch
3. Pull all from the remote repository
4. Switch back to your main branch
5. Merge the branch you just created with the main branch
6. Look for any merge conflicts and fix them
7. Once any merge conflicts are fixed, "git push -u origin [main branch]" to push your main branch to the repository
