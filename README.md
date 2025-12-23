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





