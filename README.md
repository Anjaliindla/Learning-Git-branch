# Learning-Git-branch

 Level 1: Introduction to Git Commits

This level introduces the most fundamental concept in Git: **commits**.
A commit represents a snapshot of the project at a specific point in time.
Each commit has a unique ID and forms a linear history.

You learn how Git records changes and moves the `HEAD` pointer after each commit.
<img width="1920" height="1020" alt="Screenshot 2025-12-17 105917" src="https://github.com/user-attachments/assets/2337d4ad-c0f0-4edf-bff8-9a0d265554aa" />

 Commands Used

```bash
git commit
git commit
```

 Level 2: Branching in Git

This level explains **branches**, which allow you to work on different versions of a project independently.
A new branch is created from an existing commit, and you can switch between branches using checkout.

Here, a `bugfix` branch is created from `main` and checked out.

<img width="1920" height="1020" alt="Screenshot 2025-12-17 110312" src="https://github.com/user-attachments/assets/df4d9f61-393f-4e1c-a090-c114f0040bd6" />


 Commands Used

```bash
git branch bugfix
git checkout bugfix
```

 Level 3: Merging in Git

This level demonstrates how to **merge branches**.
You first make commits on the `bugfix` branch, then switch back to `main`, add another commit, and finally merge `bugfix` into `main`.

Merging combines the histories of two branches and may create a **merge commit**.
<img width="1920" height="1020" alt="Screenshot 2025-12-17 110452" src="https://github.com/user-attachments/assets/cb639a1f-2def-4258-989a-57680d154d63" />


 Commands Used

```bash
git branch bugfix
git checkout bugfix
git commit
git checkout main
git commit
git merge bugfix
```

 Level 4: Rebase Introduction


This level introduces **rebasing**, an alternative to merging.
Rebasing moves the commits from one branch and replays them on top of another branch, creating a **linear history**.

Here, commits from `bugfix` are rebased onto `main`.

<img width="1920" height="1020" alt="Screenshot 2025-12-17 110714" src="https://github.com/user-attachments/assets/737e156d-bcfb-44b6-9c54-c4ae052f7839" />


 Commands Used

```bash
git branch bugfix
git checkout bugfix
git commit
git checkout main
git commit
git checkout bugfix
git rebase main
```

LEVEL - 2

 Level 1: Detach `HEAD`

In this level, you learn about **detached HEAD state**.
Normally, `HEAD` points to a branch. When you checkout a specific commit instead of a branch, `HEAD` becomes detached and points directly to that commit.

This is useful for:

* Inspecting old commits
* Debugging without affecting branches

 <img width="1920" height="1020" alt="Screenshot 2025-12-17 110951" src="https://github.com/user-attachments/assets/52ebe8f5-2f0e-4fa4-9a6b-03a3134f1079" />


 Commands Used

```bash
git branch bugfix
git checkout c4
```


 Level 2: Relative Refs (`^`)


This level introduces **relative references** using the caret (`^`) operator.
The `^` symbol means “parent commit”.

<img width="1920" height="1020" alt="Screenshot 2025-12-17 111057" src="https://github.com/user-attachments/assets/758bfd2c-d521-4a4b-bb0e-7c783f7bcf47" />


 Commands Used

```bash
git checkout c3
```


 Level 3: Relative Refs #2 (`~`)


This level focuses on the tilde (`~`) operator and **forcing branches** to point to specific commits.

Examples:

* `HEAD~1` → one commit before HEAD
* `HEAD~2` → two commits before HEAD

You also learn how to **move branches forcibly**.
<img width="1920" height="1020" alt="Screenshot 2025-12-17 112603" src="https://github.com/user-attachments/assets/ecf76393-4db1-4047-94bc-6a1b9099c80e" />


 Commands Used

```bash
git checkout HEAD~1
git branch -f main c6
git branch -f bugfix c0
```


 Level 4: Reversing Changes in Git


This level teaches how to **undo changes safely and unsafely** using `reset` and `revert`.

<img width="1920" height="1020" alt="Screenshot 2025-12-23 110525" src="https://github.com/user-attachments/assets/b4b37725-a9d6-4005-87ee-817a7f78ea89" />


 Commands Used

```bash
git checkout local
git reset --hard c1
git checkout pushed
git revert pushed
```








