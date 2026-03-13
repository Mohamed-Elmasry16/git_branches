# Git Branches Lab

## Project Description

This repository demonstrates essential **Git and GitHub workflow operations** such as creating repositories, managing branches, merging changes, and tagging releases.

The project was created as part of a lab exercise to practice real-world version control tasks using Git.

---

# Technologies Used

* Git
* GitHub

---

# Repository Workflow

The workflow implemented in this repository includes:

1. Creating a local Git repository.
2. Connecting the local repository to a remote GitHub repository.
3. Creating multiple branches.
4. Adding files to different branches.
5. Merging branches into the main branch.
6. Creating an annotated version tag.

---

# Project Structure

```
git_branches
│
├── README.md
├── dev.txt
└── test.txt
```

---

# Branch Structure

```
main
 ├── dev
 └── test
```

* **main** → production branch
* **dev** → development branch
* **test** → testing branch

---

# Steps Implemented

## 1. Initialize Local Repository

```
git init
```

---

## 2. Connect to Remote Repository

```
git remote add origin https://github.com/username/git_branches.git
git branch -M main
git push -u origin main
```

---

## 3. Create Development Branch

```
git checkout -b dev
```

Add a file:

```
echo "This file belongs to dev branch" > dev.txt
git add .
git commit -m "Add dev file"
git push origin dev
```

---

## 4. Create Test Branch

```
git checkout main
git checkout -b test
```

Add a file:

```
echo "This file belongs to test branch" > test.txt
git add .
git commit -m "Add test file"
git push origin test
```

---

## 5. Merge Branches

Merge branches into the main branch:

```
git checkout main
git merge dev
git merge test
git push origin main
```

---

## 6. Create Annotated Tag

```
git tag -a v1.7 -m "Version 1.7 release"
```

---

## 7. Push Tag

```
git push origin v1.7
```

---

# Version

Current release:

```
v1.7
```

---

# Author

**Mohamed Walled Ezzat**
ML/AI Engineer
Email: [mwezzat16@gmail.com](mailto:mwezzat16@gmail.com)
