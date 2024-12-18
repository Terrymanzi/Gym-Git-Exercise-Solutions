# Gym-Git-Exercise-Solutions

## BUNDLE 1
### EXERCISE 1 (terminal history)
```bash
Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1
$ git init
Initialized empty Git repository in C:/Users/Terry/Desktop/The Gym Program/Learning/Git Learning/project_1/.git/

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (main)
$ touch index.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (main)
$ ls
index.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (main)
$ touch style.css

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (main)
$ git branch -m master main
fatal: no branch named 'master'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (main)
$ git branch -m main master

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ gti branch
bash: gti: command not found

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git branch

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git add .

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git commit -m "first commit with project files on master branch"
[master (root-commit) 1dd3b34] first commit with project files on master branch
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
 create mode 100644 style.css

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git remote add origin https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git remote -v
origin  https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git (push)

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 252 bytes | 126.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions/pull/new/master
remote:
To https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (master)
$ git checkout -b dev
Switched to a new branch 'dev'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git checkout -b test
Switched to a new branch 'test'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (test)
$ git checkout dev
Switched to branch 'dev'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git branch -d test
Deleted branch test (was 1dd3b34).

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git push -u origin master
Everything up-to-date
branch 'master' set up to track 'origin/master'.

```

### EXERCISE 2 (terminal history)
```bash
Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ touch home.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ ls
home.html  index.html  style.css

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ vi home.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git add home.html
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ gti stash save "home.html changes"
bash: gti: command not found

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash save "home.html changes"
Saved working directory and index state On dev: home.html changes

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ vi about.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git add about.html
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash save "about.html changes"
Saved working directory and index state On dev: about.html changes

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ vi team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git add team.html
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash save "team.html changes"
Saved working directory and index state On dev: team.html changes

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stack pop
git: 'stack' is not a git command. See 'git --help'.

The most similar commands are
        stage
        stash

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (c965b4062c0cdd8cff8e3a8a05930aca1e88e22f)

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash list
stash@{0}: On dev: about.html changes
stash@{1}: On dev: home.html changes

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html
        new file:   team.html

Dropped stash@{1} (f6f243c0eee31ead9de4547552a057515afc5e20)

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git add home.html about.html
fatal: pathspec 'about.html' did not match any files

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ ls
home.html  index.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash list
stash@{0}: On dev: about.html changes

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (e82f7f1b19991966d30cec1d173133332138fc99)

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ ls
about.html  home.html  index.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git add about.html home.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git commit -m "added home and about pages to dev branch"
[dev 23c580a] added home and about pages to dev branch
 3 files changed, 16 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git push origin master
Everything up-to-date

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git push origin dev
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 583 bytes | 291.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git reset HEAD team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git checkout -- team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git status
On branch dev
nothing to commit, working tree clean

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$

```

## BUNDLE 2
### EXERCISE 1 (terminal history)
```bash
Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/bundle-2)
$ vi services.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/bundle-2)
$ ls
about.html  home.html  index.html  services.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/bundle-2)
$ git add services.html
warning: in the working copy of 'services.html', LF will be replaced by CRLF the next time Git touches it

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/bundle-2)
$ git commit -m "added services.html with some content"
[ft/bundle-2 f3bb7df] added services.html with some content
 1 file changed, 4 insertions(+)
 create mode 100644 services.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 402 bytes | 402.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

```

### EXERCISE 2 (terminal history)
```bash

```

## BUNDLE 3
### EXERCISE 1 (terminal history)
```bash

```

### EXERCISE 2 (terminal history)
```bash

```

## BUNDLE 4
### EXERCISE 1 (terminal history)
```bash

```

### EXERCISE 2 (terminal history)
```bash

```


## BUNDLE 5
### EXERCISE 1 (terminal history)
```bash

```

### EXERCISE 2 (terminal history)
```bash

```


## BUNDLE 6
### EXERCISE 1 (terminal history)
```bash

```

### EXERCISE 2 (terminal history)
```bash

```
### EXERCISE 3 (terminal history)
```bash

```
### EXERCISE 4 (terminal history)
```bash

```








