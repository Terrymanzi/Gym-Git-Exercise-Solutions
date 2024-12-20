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

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign)
$ ls
README.md  about.html  home.html  index.html  services.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign)
$ git diff main
diff --git a/services.html b/services.html
index d55881c..b8dee02 100644
--- a/services.html
+++ b/services.html
@@ -1,4 +1,4 @@
 <html>
   <head><title>Services</title></head>
-  <body><h1>Our Services</h1><p>Explore the variety of services we now offer, including our new premium options.</p></body>
+  <body><h1>Our Updated Services</h1><p>We have restructured our services to provide better value.</p></body>
 </html>

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ vi services.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ git merge main
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ vi services.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ git merge main
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ vi services.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ git merge main
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ git add servies.html
fatal: pathspec 'servies.html' did not match any files

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ ls
README.md  about.html  home.html  index.html  services.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ git add services.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign|MERGING)
$ git commit -m "resolved conflicts and merged main into ft/service-redesign"
[ft/service-redesign 09ae2d5] resolved conflicts and merged main into ft/service-redesign

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 245 bytes | 245.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git
   1b701eb..09ae2d5  ft/service-redesign -> ft/service-redesign

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/service-redesign)
$
```

## BUNDLE 3
### EXERCISE 1 (terminal history)
```bash

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ ls
README.md  about.html  home.html  index.html  services.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ cat team.html
<html>
  <head><title>Team</title></head>
  <body><h1>Meet our Team</h1></body>
</html>

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (main)
$ git checkout -b ft/contact-page
fatal: a branch named 'ft/contact-page' already exists

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (main)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git log
commit f2002e1ff5b85c0a309bfbc51ec56ba211262105 (HEAD -> ft/team-page, origin/ft/team-page)
Author: terrymanzi <m.terry@alustudent.com>
Date:   Wed Dec 18 17:58:41 2024 +0200

    modified team.html page content

commit 09ae2d5246896b41d2ee6a318cc55017f5c5ed82 (origin/ft/service-redesign, ft/service-redesign)
Merge: 1b701eb 5fbc0fa
Author: terrymanzi <m.terry@alustudent.com>
Date:   Wed Dec 18 17:48:17 2024 +0200

    resolved conflicts and merged main into ft/service-redesign

commit 5fbc0fa761ca7ea0012c659d71955dc558819026 (origin/main, origin/HEAD, main)
Author: terrymanzi <m.terry@alustudent.com>
Date:   Wed Dec 18 13:58:47 2024 +0200

    updated services page with new content

commit 1b701ebc0e22e89e4f1cfe3c02b1561881b2b88b
Author: terrymanzi <m.terry@alustudent.com>
Date:   Wed Dec 18 13:40:35 2024 +0200

    redesigned the services.html page

commit a35adb3f96c79f6b754886ffe38764b824bcb123
Merge: 883c85e f3bb7df
Author: Terry <156342254+Terrymanzi@users.noreply.github.com>
Date:   Wed Dec 18 13:31:55 2024 +0200

    Merge pull request #1 from Terrymanzi/ft/bundle-2

    Add services.html page

commit 883c85ee79531609d7b428b96649c468270ba4ed
Author: Terry <156342254+Terrymanzi@users.noreply.github.com>
Date:   Wed Dec 18 13:31:14 2024 +0200

    done exercise 1 in bundle 2 (README.md)

commit 442eceb360f6c45531898af4c5e8968e18115d02
Author: Terry <156342254+Terrymanzi@users.noreply.github.com>
Date:   Wed Dec 18 13:19:58 2024 +0200

    Updated README.md

commit d86bf740fd49e2a1c3eed4b0754599be01f52b21
Author: Terry <156342254+Terrymanzi@users.noreply.github.com>
Date:   Wed Dec 18 12:27:47 2024 +0200

    Created and updated README.md


Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git cherry-pick f2002e1ff5b85c0a309bfbc51ec56ba211262105
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit f2002e1.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --continue
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit f2002e1.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page|CHERRY-PICKING)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
warning: cancelling a cherry picking in progress
Your branch is up to date with 'origin/ft/team-page'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git push -u origin ft/team-page
Everything up-to-date
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ ls
README.md  about.html  contact.html  home.html  index.html  services.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ cat contact.html
<html>
        <head>
                <title>Contact</title>
        </head>
        <body>
                <h1>Contact Us</h1>
        </body>
</html>

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ vi contact.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git add contact.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git commit -m "I added contact.html page with some content"
On branch ft/contact-page
nothing to commit, working tree clean

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git push -u origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 672 bytes | 67.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git checout -b ft/faq-page
git: 'checout' is not a git command. See 'git --help'.

The most similar command is
        checkout

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ ls
README.md  about.html  contact.html  home.html  index.html  services.html  style.css  team.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ echo "<html><head><title>FAQ</title></head><body><h1>Frequently Asked Questions</h1></body></html>" > faq.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ cat faq.html
<html><head><title>FAQ</title></head><body><h1>Frequently Asked Questions</h1></body></html>

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ vi faq.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ git add faq.html
warning: in the working copy of 'faq.html', LF will be replaced by CRLF the next time Git touches it

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ git commit -m "Added the faq.html page"
[ft/faq-page 0c5aa24] Added the faq.html page
 1 file changed, 6 insertions(+)
 create mode 100644 faq.html

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ git push -u origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 360 bytes | 360.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ gti checkout ft/team-page
bash: gti: command not found

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git revert f2002e1ff5b85c0a309bfbc51ec56ba211262105
[ft/team-page f049fbb] Revert "modified team.html page content"
 1 file changed, 1 insertion(+), 1 deletion(-)

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git psuh
git: 'psuh' is not a git command. See 'git --help'.

The most similar command is
        push

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 356 bytes | 356.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Terrymanzi/Gym-Git-Exercise-Solutions.git
   f2002e1..f049fbb  ft/team-page -> ft/team-page

Terry@DESKTOP-MAAMI2P MINGW64 ~/Desktop/The Gym Program/Learning/Git Learning/project_1 (ft/team-page)
$

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








