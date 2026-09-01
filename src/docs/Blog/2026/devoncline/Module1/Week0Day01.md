# Week 0 - Day 1

## Computational Thinking, A Coder's Computer, and Git

---

# Computational Thinking

Computational thinking is a way of breaking down problems so they can be solved logically.

## Decomposition

**Definition:** Break a large problem into smaller, easier tasks.

Instead of trying to solve one huge problem at once, divide it into smaller problems that can be worked on individually.

---

## Pattern Recognition

**Definition:** Notice similarities, repetition, or patterns that can help solve a problem.

If a problem looks similar to something that has already been solved, the same general approach may work again.

---

## Abstraction

**Definition:** Ignore unnecessary details and focus on the important parts of a problem.

This helps simplify complicated problems by concentrating on what actually matters to the solution.

---

## Algorithmic Thinking

**Definition:** Determine the exact steps necessary to accomplish a goal.

Example:

1. Receive an input.
2. Perform a set of instructions.
3. Produce an output.

---

## Debugging

**Definition:** Find, analyze, and fix errors.

A basic debugging process:

1. Reproduce the problem.
2. Determine where it is happening.
3. Find the cause.
4. Make a change.
5. Test again.

Debugging is not only fixing error messages. It also includes figuring out why a program behaves differently than expected.

---

# Algorithms

An **algorithm** is a defined series of steps used to produce a result.

A simple model:

**Input → Instructions/Steps → Output**

## Characteristics of a Good Algorithm

### Well-Defined Input

The algorithm should clearly know what information it receives.

### Well-Defined Output

The expected result should be clear.

### Clear / Unambiguous

Each instruction should have one specific meaning.

### Finite

The algorithm must eventually stop.

### Feasible

Every step must actually be possible to perform.

### Language Independent

An algorithm is the **idea or procedure**, not the programming language.

The same algorithm could be implemented in:

* JavaScript
* TypeScript
* Python
* C#
* Java

The syntax changes, but the algorithm itself can remain the same.

---

# Variables

A **variable** is a named place for storing a value.

Example:

```text
age = 25
name = "Devon"
isStudent = true
```

Variables can hold different kinds of data.

## String

Text.

```text
name = "Devon"
```

## Number

```text
age = 25
```

## Boolean

A value that is either true or false.

```text
isStudent = true
```

---

# Control Structures

Control structures determine **which instructions run and how often they run**.

## Conditionals

Conditionals allow a program to make decisions.

Conceptually:

```text
IF condition is true
    do something
ELSE
    do something else
```

---

## Loops / Iteration

Loops repeat instructions.

Instead of:

```text
display item 1
display item 2
display item 3
display item 4
```

A program can conceptually do:

```text
FOR every item
    display item
```

---

## `break`

Stops a loop completely.

## `continue`

Skips the current item and moves to the next one.

---

# Data Structures

A **data structure** is a way of organizing information so a program can work with it.

## List / Array

A collection of items.

```text
items = [
    Item A,
    Item B,
    Item C
]
```

---

## Object / Dictionary

Stores related information using keys and values.

Conceptually:

```text
person
    name = "Devon"
    age = 25
    student = true
```

Which can also be thought of as:

```text
name → Devon
age → 25
student → true
```

---

## Set

A collection where each value is unique.

Example input:

```text
red
blue
red
green
blue
```

A Set would contain:

```text
red
blue
green
```

---

# Version Control

**Version control** is the general idea of tracking changes to files over time.

It allows developers to:

* Keep a history of changes
* Return to older versions
* Experiment safely
* Collaborate with other developers
* Track who changed what

---

# Git

**Git** is a distributed version control system.

Git can track:

* Repositories
* Files
* Commits
* Branches
* Merges
* Project history

Because Git is **distributed**, developers can have complete local repositories and histories on their own computers.

---

# Git vs. GitHub

## Git

Git is the actual version control software.

It handles things such as:

* Commits
* Branches
* Merges
* Staging
* History
* Local repositories

## GitHub

GitHub is an online service that hosts Git repositories.

GitHub helps with:

* Backing up repositories
* Sharing code
* Collaboration
* Remote repositories

Other platforms mentioned in the lesson that work with Git include:

* GitLab
* Bitbucket

### Easy Reminder

> **Git = version control**

> **GitHub = online hosting/collaboration for Git repositories**

---

# Other Version Control Systems

Git is not the only version control system.

The lesson also mentioned:

* Subversion (SVN)
* Mercurial
* CVS
* Bazaar

These are alternatives to Git, not programs that use Git.

## Git vs. SVN

**Git = distributed**

**SVN = centralized**

With Git, each developer can have their own complete local repository.

With SVN, development is centered around one central repository.

---

# Repository

A **repository**, or **repo**, is a project that Git is tracking along with its version history.

A normal folder contains its current files.

A Git repository contains:

> **Current files + Git history**

---

# `git init`

```bash
git init
```

**init = initialize**

Turns a normal folder into a Git repository.

Conceptually:

```text
Normal Folder
     ↓
  git init
     ↓
Git Repository
```

Opening a folder in VS Code does **not** automatically make it a Git repository.

If a project was cloned from an existing repository, `git init` is not necessary because the cloned folder is already a Git repository.

---

# `git clone`

```bash
git clone <repository-url>
```

Creates a local copy of an existing Git repository.

Cloning brings down things such as:

* Project files
* Git history
* Branch information
* Remote connection

GitHub Desktop can also perform a clone through its interface instead of requiring the terminal command.

---

# Commits

A **commit** is a snapshot or checkpoint in the history of a Git repository.

Example history:

```text
Initial project
↓
Add homepage
↓
Add login
↓
Fix login bug
```

Each commit represents another point in the project's history.

### Save vs. Commit

`Ctrl + S` saves the current file.

A **Git commit** records a checkpoint in the project's Git history.

These are not the same thing.

---

# Staging and `git add`

Changing a file does not automatically place it into the next commit.

The general process is:

```text
Changed
↓
Staged
↓
Committed
```

## `git add`

```bash
git add filename
```

Means:

> Include this change in my next commit.

Example:

```bash
git add README.md
```

Another common command is:

```bash
git add .
```

which can stage multiple changes.

---

# `git status`

```bash
git status
```

Shows the current state of the repository.

It can show:

* Current branch
* Modified files
* Staged files
* Untracked files
* Whether the local branch is ahead or behind

`git status` is safe to run because it does not change anything.

Think:

> **"Git, tell me what's going on."**

---

# `git push`

```bash
git push
```

Sends local commits to the remote repository.

Usually:

```text
My Computer → GitHub
```

### Memory Trick

**Push = push changes away from my computer.**

---

# `git pull`

```bash
git pull
```

Brings newer remote changes down and integrates them into the local repository.

Usually:

```text
GitHub → My Computer
```

### Memory Trick

**Pull = pull changes toward my computer.**

---

# Branches

A **branch** is a separate line of development.

Conceptually:

```text
main
│
├── feature-one
├── feature-two
└── experiment
```

A developer can work on another branch without immediately changing `main`.

Once the work is ready, it can be merged.

---

# Merge

A **merge** combines changes from one branch into another.

Example:

```text
main
  \
   \── feature
         ↓
       work
         ↓
       merge
         ↓
main contains the feature
```

---

# Merge Conflicts

Git can automatically combine many changes.

A **merge conflict** happens when Git cannot safely determine how two versions should be combined.

Example:

One developer changes a line to:

```text
Welcome back
```

Another developer changes the same line to:

```text
Good morning
```

Git cannot know which result is correct.

A developer must decide whether to:

* Keep the first version
* Keep the second version
* Combine both
* Write a new final version

> Git identifies the conflict. Humans determine the correct final code.

---

# Basic Collaboration Workflow

When several people are working on the same project:

```text
Pull latest changes
↓
Work
↓
Commit
↓
Pull again if others may have pushed
↓
Resolve conflicts if necessary
↓
Test
↓
Push
```

If the remote branch contains commits that the local branch does not have, Git will normally reject a regular push until the local repository is updated.

This helps prevent developers from accidentally overwriting one another's normal commits.

---

# Force Push

A force push can rewrite remote Git history.

Example:

```bash
git push --force
```

This can be dangerous on shared branches such as `main`.

Avoid force pushing shared branches unless there is a specific reason and the team understands what is happening.

---

# `origin`

`origin` is usually Git's nickname for the remote repository associated with a local repository.

Conceptually:

```text
origin → remote GitHub repository
```

Example:

```bash
git push origin main
```

Means roughly:

> Push my `main` branch to the remote repository called `origin`.

---

# Git Configuration

Git can attach a name and email to commits.

## Global Username

```bash
git config --global user.name "Devon Cline"
```

`--global` means the setting becomes the default for Git repositories on that computer.

Check it with:

```bash
git config --global user.name
```

A specific repository can also have a local setting that overrides the global setting.

---

# Useful Git Commands From Day 1

```bash
git init
```

Initialize a Git repository.

```bash
git clone <url>
```

Clone an existing repository.

```bash
git status
```

See the current repository status.

```bash
git add <file>
```

Stage a change.

```bash
git commit -m "message"
```

Create a commit.

```bash
git pull
```

Bring remote changes down.

```bash
git push
```

Send local commits to the remote.

```bash
git checkout <branch>
```

Switch branches or versions.

```bash
git merge <branch>
```

Merge another branch into the current branch.

```bash
git log
```

View commit history.

---

# Command Flags From Day 1

## `-m`

**Message**

```bash
git commit -m "Add feature"
```

Adds a message describing the commit.

---

## `-b`

Used with checkout to create a new branch.

```bash
git checkout -b new-feature
```

Creates and switches to `new-feature`.

---

## `-a`

Can tell `git commit` to automatically include modifications to already tracked files.

---

## `-p`

**Patch**

```bash
git add -p
```

Allows only selected pieces of changes to be staged.

This is more advanced and does not need to be memorized yet.

---

# Terminal Navigation

The terminal has its own **current working directory**.

## `pwd`

```bash
pwd
```

**Print Working Directory**

Shows the terminal's current location.

## `cd ..`

```bash
cd ..
```

Moves up one folder.

## `cd FolderName`

```bash
cd FolderName
```

Moves into a folder.

The folder currently displayed in VS Code and the terminal's current location can be different.

---

# My Personal QTR4 Connections

> These are personal examples from my QTR4 project that help me connect the class terminology to things I have already worked with.

## Decomposition

When I work on a large QTR4 feature such as Packs, I can break it into smaller problems:

* Creating a pack
* Adding beats
* Selecting recipients
* Generating share links
* Loading analytics
* Deleting packs
* Handling loading states

Instead of thinking **"build Packs,"** I can think about each smaller problem individually.

---

## Pattern Recognition

I have seen similar problems appear in different parts of QTR4.

For example, Vault and Packs have both needed things such as:

* Pagination
* Loading states
* Empty states
* Sorting
* Infinite scrolling

If I recognize that two features have similar problems, I may be able to use a similar solution.

---

## Abstraction

For something like favoriting a beat, I can temporarily ignore database details and UI styling.

The core problem is simply:

> A user clicks a star and the favorite state changes.

Once that works, the smaller details can be added.

---

## Algorithms

Favoriting a beat can be thought of as an algorithm:

```text
User clicks favorite
↓
Identify the beat
↓
Check current favorite state
↓
Favorite or unfavorite it
↓
Save the result
↓
Update the UI
```

My Packs infinite scrolling also follows an algorithm:

```text
User reaches bottom
↓
Check if more packs exist
↓
Request next page
↓
Add the returned packs
↓
Update whether more packs remain
```

---

## Variables

Variables I recognize from the kinds of code I've seen in QTR4 include concepts like:

```text
isLoading
hasMore
searchQuery
pageSize
isFavorited
userId
selectedPack
```

These are names that hold information the program needs while running.

---

## Control Structures

A QTR4 conditional might conceptually be:

```text
IF hasMore
    load more packs
ELSE
    stop loading
```

Another:

```text
IF beat is favorited
    unfavorite it
ELSE
    favorite it
```

---

## Loops

QTR4 frequently needs to repeat an operation for collections of:

* Beats
* Packs
* Tags
* Notifications
* Search results
* Recipients

Instead of manually displaying each item, the program loops through a collection.

---

## Data Structures

A list of beats is an example of a collection/data structure.

One beat can also contain related information such as:

```text
title
BPM
key
tags
favorite status
created date
```

This helps me understand the difference between **one object** and a **collection of objects**.

---

## Repository

My QTR4 project is not only a folder of source code.

It is also a **Git repository**, meaning Git stores a history of the changes made to the project.

---

## Commits

When I finish a QTR4 change and make a commit, I am creating a checkpoint in the project's history.

Example:

```text
Add feature
↓
Fix loading state
↓
Improve analytics
↓
Fix bug
```

These commits make it possible to see how the project changed over time.

---

## `git add` and VS Code Source Control

I usually do not manually type:

```bash
git add
```

for QTR4.

VS Code's Source Control interface handles the staging workflow visually.

Conceptually:

```text
I edit a file
↓
It appears under Changes
↓
It gets staged
↓
I commit
```

Clicking the **+** beside a changed file in VS Code is similar to running:

```bash
git add filename
```

---

## Push, Pull, and Sync Changes

My normal QTR4 workflow has often been:

```text
Make changes
↓
Commit
↓
Sync Changes
```

VS Code is providing a graphical interface around Git operations.

### Push

```text
My QTR4 commits → GitHub
```

### Pull

```text
GitHub updates → My local QTR4 repository
```

Because I normally work solo from one computer, I have not needed to think about `git pull` very often.

It would become more important if:

* I worked from multiple computers
* Someone else worked on QTR4
* I changed code directly on GitHub
* A remote pull request was merged

---

## Branches

I mostly work from `main`, but a branch could allow me to work on something like:

```text
main
│
├── favorites-feature
├── social-page
└── packs-redesign
```

without immediately changing the main version of QTR4.

---

## Merge Conflicts

I have mostly worked solo, so I have not dealt with many true collaboration conflicts yet.

If another developer and I both changed the same part of QTR4 differently, Git might not know which version to keep.

Git would identify the conflict, and we would have to decide what the correct final code should be.

---

# My Day 1 Mental Model

## Programming Concepts

```text
Problem
↓
Break it down
↓
Find patterns
↓
Create an algorithm
↓
Use variables + control structures + data structures
↓
Debug when behavior is wrong
```

## Git

```text
Edit
↓
Stage
↓
Commit locally
↓
Pull newer remote work if needed
↓
Push
↓
GitHub
```

### Quick Reminders

> **Git = version control**

> **GitHub = hosting/collaboration for Git repositories**

> **Repository = project + Git history**

> **Commit = checkpoint**

> **Branch = separate line of development**

> **Push = local → remote**

> **Pull = remote → local**

> **Merge conflict = Git needs a human to decide the correct final version**
