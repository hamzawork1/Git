### **🚀 Git Command Cheat Sheet**

#### **🟢 Basic Setup & Configuration**

| **Command**                                        | **Description**                      |
| -------------------------------------------------- | ------------------------------------ |
| `git --version`                                    | Check installed Git version..        |
| `git config --global user.name "Your Name"`        | Set global username for Git.         |
| `git config --global user.email "you@example.com"` | Set global email for Git.            |
| `git config --global color.ui auto`                | Enable color output in Git commands. |
| `git config --list`                                | View all global Git configurations.  |

---

#### **📂 Initializing & Cloning**

| **Command**                        | **Description**                                                                                                                    |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `git init`                         | Initialize a new Git repository.                                                                                                   |
| `git clone <repo_url>`             | Clone a remote repository locally.                                                                                                 |
| `git remote add origin <repo_url>` | Set the origin of remote repository. you change name of origin instead of origin. **it helps to link local repo with remote repo** |
| `git remote -v`                    | to verify remote repository for fetch and push                                                                                     |

---

#### **📄 Staging & Committing**

| **Command**                           | **Description**                                                |
| ------------------------------------- | -------------------------------------------------------------- |
| `git status`                          | Check the status of files in the working directory.            |
| `git add <file>`                      | Stage a specific file for commit.                              |
| `git add .`                           | Stage all modified & new files.                                |
| `git commit -m "Commit message"`      | Commit staged files with a message. "its the record of change" |
| `git commit --amend -m "New message"` | Edit the last commit message.                                  |

---

#### **📤 Pushing & Pulling**

| **Command**                   | **Description**                                                                                            |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `git push origin <branch>`    | Push commits to a                                                                                          |
| `git push -u origin <branch>` | Push and set upstream tracking. **if you don't want you origin in command again & again you can use `-u`** |
| `git pull origin <branch>`    | Fetch and merge changes from remote.                                                                       |
| `git fetch`                   | Fetch changes without merging                                                                              |

---

#### **🔄 Branching & Merging**

| **Command**                | **Description**                               |
| -------------------------- | --------------------------------------------- |
| `git branch`               | List all branches.                            |
| `git branch <branch-name>` | Create a new branch.                          |
| `git branch -M <branch-name>` | Rename a branch.                          |
| `git switch <branch>`      | Switch to an existing branch.                 |
| `git checkout -b <branch>` | Create and switch to a new branch.            |
| `git merge <branch>`       | Merge a branch into the current branch.       |
| `git rebase <branch>`      | Reapply commits from one branch onto another. |

---

#### **⚔️ Resolving Merge Conflicts**

|**Command**|**Description**|
|---|---|
|`git diff <branch>`|compare commits,branhes,files & more. "before merge"|
|`git merge <branch>`|Attempt to merge branches.|
|`git status`|Check which files have conflicts.|
|`git add <file>`|Mark a conflict as resolved.|
|`git merge --abort`|Cancel a merge in progress.|

---

#### **↩️ Undoing Changes**

|**Command**|**Description**|
|---|---|
|`git restore <file>`|Undo unstaged changes to a file.|
|`git reset <file>`|Unstage a file before committing.|
|`git reset --soft HEAD~1`|Undo the last commit but keep changes staged.|
|`git reset --hard HEAD~1`|Undo the last commit and remove all changes.|
|`git revert <commit>`|Create a new commit that undoes a previous commit.|

---

#### **📜 Viewing History**

|**Command**|**Description**|
|---|---|
|`git log`|View commit history.|
|`git log --oneline --graph`|Compact log with branches visualization.|
|`git show <commit>`|View details of a specific commit.|
|`git reflog`|View all changes (even deleted commits).|

---

#### **📦 Stashing Work**

|**Command**|**Description**|
|---|---|
|`git stash`|Save changes temporarily.|
|`git stash list`|View stashed changes.|
|`git stash pop`|Apply and remove the latest stash.|
|`git stash apply`|Apply the latest stash but keep it.|

---

#### **🎯 Tags & Releases**

|**Command**|**Description**|
|---|---|
|`git tag`|List all tags.|
|`git tag -a v1.0 -m "Version 1.0"`|Create an annotated tag.|
|`git push origin --tags`|Push all tags to remote.|

---

#### **🚀 Advanced Git**

|**Command**|**Description**|
|---|---|
|`git cherry-pick <commit>`|Apply a specific commit to another branch.|
|`git bisect start`|Start finding the commit that introduced a bug.|
|`git worktree add <dir> <branch>`|Work with multiple branches at once.|