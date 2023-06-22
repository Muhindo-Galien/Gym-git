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
