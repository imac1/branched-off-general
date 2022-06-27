# Branched off

## Story

You've been using git for a while now. With this project, you will put your
knowledge to a test, by using only the terminal.
You will need to keep switching branches, so try to not to fall!

## What are you going to learn?

- Git basics
- Git branching
- Git rebase
- shell basics

## Tasks

1. Create your exercises by running the init script: `bash ./helper/init`.
    - Running command `git branch` results in the following.
```
conflict-feature
conflict-rebase-feature
demo
x master
merge-conflict
merge-simple
merge-undo-last
rebase-branch
rename-commit
simple-feature
undo-last
undo-last-but-one
undo-last-feature
```

2. Edit the history of your local `undo-last` branch by undoing the last commit.
    - On branch `undo-last`, running command `./helper/print_log` results in the following.
```
# No output
```

3. Edit the history of your local `rename-commit` branch by fixing the typo in the last commit.
    - On branch `rename-commit`, running command `./helper/print_log` results in the following.
```
f5c8307 (HEAD -> rename-commit) Important message
```

4. Go back in your local history on the `demo` branch to a previous commit. This is useful if you want to demo a working version.
    - On branch `demo`, running command `./helper/print_changed_files` results in the following.
```
just-works-tm.js
```

5. Integrate changes into the local `merge-simple branch` from the `simple-feature branch` local branch, it should go smoothly.
    - On branch `merge-simple branch`, running command: `./helper/print_log` results in the following.
```
348f321 (HEAD -> merge-simple, simple-feature) New feature works
```

6. Integrate changes into the `merge-conflict` branch from the `conflict-feature` local branch - there will be a conflict - but you are familiar with this by now.
    - On branch `merge-conflict`, running command: `./helper/print_log` results in the following.
```
0bcda64 (HEAD -> merge-conflict) Merge branch 'conflict-feature' into merge-conflict
e20c235 Old feature fix
deaf171 (conflict-feature) New feature works
```

7. Integrate changes into the `merge-undo-last` local branch from the `undo-last-feature` local branch. Before that though, you need to undo the last commit as it is redundant and may cause problems.
    - On branch `merge-undo-last`, running command: `./helper/print_log` results in the following.
```
d83e3e7 (HEAD -> merge-undo-last, undo-last-feature) New feature works
```

8. Integrate changes into the `rebase-branch` branch from the `conflict-rebase-feature` local branch. Use rebase.
    - On branch `rebase-branch`, running command: `./helper/print_log` results in the following.
```
30d0536 (HEAD -> rebase-branch) Old feature fix
2999d91 (conflict-rebase-feature) New feature works
```

9. Edit the history of your `undo-last-but-one` branch, keeping the last commit and removing the one before it.
    - On branch `undo-last-but-one`, running command: `./helper/print_log` results in the following.
```
51243ac (HEAD -> undo-last-but-one) WIP some progress with security
```

## General requirements

None

## Hints

- Examine the contents of the repository. There are examples of git usage in the scripts checked in here.
- You will push and pull a lot and it gets annoying if you have to retype your password all the time. Read the linked materials!
- Use `./helper/reset` to get back to the original state, if you feel that you made a mistake during an exercise.
- Your git hash - the first few characters of the `./helper/print_log` - are different from the one here.
- Make sure that you are on the correct branch when working on an exercise.

## Background materials

- <i class="far fa-exclamation"></i> [Git without password]
- <i class="far fa-exclamation"></i> [Undo things in git](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History)
- <i class="far fa-exclamation"></i> [Branches in a nutshell](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)
- <i class="far fa-exclamation"></i> [Branching and merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
- <i class="far fa-exclamation"></i> [Branch management](https://git-scm.com/book/en/v2/Git-Branching-Branch-Management)
- [Git branching and workflows]
- [Merge vs rebase]
- [Mastering git]
- <i class="far fa-book-open"></i> [Rebasing](https://git-scm.com/book/en/v2/Git-Branching-Rebasing)
- <i class="far fa-book-open"></i> [Bash guide](https://mywiki.wooledge.org/BashGuide)
