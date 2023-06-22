# Git exercises

This is all about the Gym git exercises

## Bundle 1
### Exercice 1
```bash
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint:   git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint:   git branch -m <name>
Initialized empty Git repository in /home/galien/Gym Rwanda/gym-git/.git/
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git branch -M main
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git branch
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git add .
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git commit -m "init exercise 1"
[main (root-commit) 80c5e81] init exercise 1
 1 file changed, 3 insertions(+)
 create mode 100644 README.md
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git remote add origin https://github.com/Muhindo-Galien/Gym-git.git
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 267 bytes | 267.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Muhindo-Galien/Gym-git.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git checkout -b dev
Switched to a new branch 'dev'
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git push -u origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Muhindo-Galien/Gym-git/pull/new/dev
remote: 
To https://github.com/Muhindo-Galien/Gym-git.git
 * [new branch]      dev -> dev
Branch 'dev' set up to track remote branch 'dev' from 'origin'.
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git checkout -b test
Switched to a new branch 'test'
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git push -u origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Muhindo-Galien/Gym-git/pull/new/test
remote: 
To https://github.com/Muhindo-Galien/Gym-git.git
 * [new branch]      test -> test
Branch 'test' set up to track remote branch 'test' from 'origin'.
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git checkout dev
M       README.md
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git branch -D test
Deleted branch test (was 80c5e81).

galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git push origin --delete test
To https://github.com/Muhindo-Galien/Gym-git.git
 - [deleted]         test
```
### Exercice 2
```bash
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git add .
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git stash 
Saved working directory and index state WIP on dev: 80c5e81 init exercise 1
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git add .
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git stash 
Saved working directory and index state WIP on dev: 80c5e81 init exercise 1
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git add .
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git stash 
Saved working directory and index state WIP on dev: 80c5e81 init exercise 1
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git stash list
stash@{0}: WIP on dev: 80c5e81 init exercise 1
stash@{1}: WIP on dev: 80c5e81 init exercise 1
stash@{2}: WIP on dev: 80c5e81 init exercise 1
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (fe439f994512cc825906ae0bf49e76f9e253bbc5)
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{1} (390d4867713ff67327f364010f77e7cd09ceaaef)
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git add .
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git commit -m "added home and about page"
[dev e56ad50] added home and about page
 3 files changed, 25 insertions(+), 1 deletion(-)
 create mode 100644 about.html
 create mode 100644 home.html
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git push origin dev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 611 bytes | 611.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Muhindo-Galien/Gym-git.git
   80c5e81..e56ad50  dev -> dev
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (6d55fccfaa94430a1b7490f2d730471064c4f4f0)
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git reset --hard
HEAD is now at e56ad50 added home and about page
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ 
```
## Bundle 2
### Exercice 1

```bash
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ touch services.html
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git add .
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ 'git commit -m "services page added"
> '^Ct commit -m "services page added"
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git commit -m "services page added"
[ft/bundle-2 ad6a3ca] services page added
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ git push origin ft/bundle-2 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 465 bytes | 465.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Muhindo-Galien/Gym-git/pull/new/ft/bundle-2
remote: 
To https://github.com/Muhindo-Galien/Gym-git.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
galien@galien-HP-EliteBook-Folio-9470m:~/Gym Rwanda/gym-git$ 
```
