# .git
if folder have .git file it means git tracks the changes of this folder. 
```
~# ls -a

.git
```

# Git Status

4 Type of git status:

1. untracked                   |    new files that git doesn't yet track
2. modified                     |    changed
3. staged                         |    file is ready to be committed
4. unmodified                 |    unchaged

### Flow: 
1. file change (status: modified) -> add (status: staged) -> commit (status: unchanged)
2. new file added (status: untracked) -> add (status: staged) -> commit (status: unchanged)

# filename.md `M`
In VS code in front of file name if shows `M` it means file modified. example
```
readme.md `M`
```
it means you need to commit the changes "in simple means takes the screenshot of this file"

Changes not staged for commit:
  (use "git add `<file>`..." to update what will be committed)
  (use "git restore `<file>`..." to discard changes in working directory)
	  modified:   readme.md

# filename.md `U`
In VS code in front of file name if shows `U` it means untracked file . example
```
readme1.md `U`
```
it means you need to add 
Untracked files:
  (use "git add `<file>`..." to include in what will be committed)
        readme1.md

# filename.md `A`
In VS code in front of file name if shows `A` it means file Added after `git add .`
```
readme1.md `A`
```

# Work Flow: 

### Local Git:
 GitHub-repo -> clone -> changes -> add -> commit -> push
### Best practice:
**Always create a repo on GitHub first, then clone it locally.** This avoids conflicts and simplifies setup 

# Merging code

Two ways
1. 1st way
2. 2nd way

### 1st way: 

`git diff main`
`git merge main`

### 2nd way:

**Pull request:** its lets you tell others about changes you've pushed to a branch in a repository on GitHub.


When we merge dev into main from GitHub we should also update local main branch with pull command. this command will run inside main branch.

`git checkout main`
`git pull origin main`

Check definition of pull (dev). [[Git Cheat sheet]]
