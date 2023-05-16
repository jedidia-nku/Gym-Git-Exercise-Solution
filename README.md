# Bundle 3

## Exercise 1

```bush
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b ft/team-page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b ft/team-pages
Switched to a new branch 'ft/team-pages'
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit "feat: add team page "
error: pathspec 'feat: add team page ' did not match any file(s) known to git
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "feat: add team page "
[ft/team-pages b6eb2b1] feat: add team page
 1 file changed, 2 insertions(+), 2 deletions(-)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push
fatal: The current branch ft/team-pages has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-pages

upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> ^C
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push --set-upstream origin ft/team-pages
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 296 bytes | 32.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/team-pages' on GitHub by visiting:
remote:      https://github.com/jedidia-nku/Gym-Git-Exercise-Solution/pull/new/ft/team-pages
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
branch 'ft/team-pages' set up to track 'origin/ft/team-pages'.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Aborting
On branch ft/team-pages
Your branch is up to date with 'origin/ft/team-pages'.

Changes not staged for commit:
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout mainn
error: pathspec 'mainn' did not match any file(s) known to git
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on ft/team-pages: b6eb2b1 feat: add team page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on ft/team-pages: b6eb2b1 feat: add team page
stash@{3}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop 'stash@{0}'
On branch ft/team-pages
Your branch is up to date with 'origin/ft/team-pages'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{0} (4d783a5767783604da501b3ba75a420058e0c3b0)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git status
Your branch is up to date with 'origin/ft/team-pages'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
no changes added to commit (use "git add" and/or "git commit -a")
On branch ft/team-pages
Your branch is up to date with 'origin/ft/team-pages'.

Changes not staged for commit:
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout main 
error: Your local changes to the following files would be overwritten by checkout:
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on ft/team-pages: b6eb2b1 feat: add team page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git status
On branch ft/team-pages
Your branch is up to date with 'origin/ft/team-pages'.

nothing to commit, working tree clean
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout ft/team-pages
Switched to branch 'ft/team-pages'
Your branch is up to date with 'origin/ft/team-pages'.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git log
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

commit 09b35b99147a1c431b169de1a2a8280bd7f9ea44
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:29:06 2023 +0200

    feat: add service list

commit 43213ecefb37c9e4f61d94098c9711e0e564f08e (origin/main)
Merge: 26a223a fd781a5
Author: Jedidia Nkunzumwami <131678447+jedidia-nku@users.noreply.github.com>
Date:   Mon May 15 00:01:05 2023 +0200

    Merge pull request #1 from jedidia-nku/ft/team-page

commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

commit 09b35b99147a1c431b169de1a2a8280bd7f9ea44
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:29:06 2023 +0200

    feat: add service list

commit 43213ecefb37c9e4f61d94098c9711e0e564f08e (origin/main)
Merge: 26a223a fd781a5
Author: Jedidia Nkunzumwami <131678447+jedidia-nku@users.noreply.github.com>
Date:   Mon May 15 00:01:05 2023 +0200

    Merge pull request #1 from jedidia-nku/ft/team-page


    
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

...skipping...
    Add new html pages to the project

commit fd781a5fd33264e9b7cf31d1c74ba9c28bde7d5f (origin/ft/team-page, ft/team-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 23:44:36 2023 +0200

    create the service page

commit 87747721affa059558519bde537f250ac24940c1 (origin/dev, dev)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 22:45:14 2023 +0200

    set up the home and about page

commit 26a223a2df8a1c427044f166e17536a089e26225
Author: Jedidia Nkunzumwami <didiernkunzumwami@gmail.com>
Date:   Sun May 14 17:45:38 2023 +0200

    This is the exercise one of bundle one
...skipping...
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

...skipping...
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

...skipping...

    Add new html pages to the project

commit fd781a5fd33264e9b7cf31d1c74ba9c28bde7d5f (origin/ft/team-page, ft/team-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 23:44:36 2023 +0200

    create the service page

commit 87747721affa059558519bde537f250ac24940c1 (origin/dev, dev)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 22:45:14 2023 +0200

    set up the home and about page

commit 26a223a2df8a1c427044f166e17536a089e26225
Author: Jedidia Nkunzumwami <didiernkunzumwami@gmail.com>
Date:   Sun May 14 17:45:38 2023 +0200

...skipping...

commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

commit 09b35b99147a1c431b169de1a2a8280bd7f9ea44
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:29:06 2023 +0200
...skipping...
    Add new html pages to the project

commit fd781a5fd33264e9b7cf31d1c74ba9c28bde7d5f (origin/ft/team-page, ft/team-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 23:44:36 2023 +0200

    create the service page

commit 87747721affa059558519bde537f250ac24940c1 (origin/dev, dev)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 22:45:14 2023 +0200

    set up the home and about page

commit 26a223a2df8a1c427044f166e17536a089e26225
Author: Jedidia Nkunzumwami <didiernkunzumwami@gmail.com>
Date:   Sun May 14 17:45:38 2023 +0200

    This is the exercise one of bundle one
...skipping...
commit b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 (HEAD -> ft/team-pages, origin/ft/team-pages)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

...skipping...
    Add new html pages to the project

commit fd781a5fd33264e9b7cf31d1c74ba9c28bde7d5f (origin/ft/team-page, ft/team-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 23:44:36 2023 +0200

    create the service page

commit 87747721affa059558519bde537f250ac24940c1 (origin/dev, dev)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Sun May 14 22:45:14 2023 +0200

    set up the home and about page

commit 26a223a2df8a1c427044f166e17536a089e26225
Author: Jedidia Nkunzumwami <didiernkunzumwami@gmail.com>
Date:   Sun May 14 17:45:38 2023 +0200

    This is the exercise one of bundle one
...skipping...
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page

commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Merge: 09b35b9 f652622
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200

    feat: add old services

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git log
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 13:13:05 2023 +0200

    feat: add team page
commit 1493b26f241ae35dc25f77ae7a433c52bbbb8cff (origin/ft/service-redesign, ft/service-redesign)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 12:00:22 2023 +0200

commit f6526226f9c04d8ad8db596b096426f39d19e5f6 (main, ft/contact-page)
Author: Jedidia-nku <didiernkunzumwami@gmail.com>
Date:   Tue May 16 11:43:32 2023 +0200
    feat: add old services

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git check ft/contact-page
git: 'check' is not a git command. See 'git --help'.

The most similar command is
        checkout
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout ft/contact-page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git cherry-pick b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0
[ft/contact-page 071337c] feat: add team page
 Date: Tue May 16 13:13:05 2023 +0200
 1 file changed, 2 insertions(+), 2 deletions(-)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add contact.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "feat: add a contact page"
[ft/contact-page ce029ed] feat: add a contact page
 1 file changed, 12 insertions(+)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> push --set-upstream origin ft/contact-page
push : The term 'push' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if a path    
was included, verify that the path is correct and try again.
At line:1 char:1
+ push --set-upstream origin ft/contact-page
    + CategoryInfo          : ObjectNotFound: (push:String) [], CommandNotFoundException
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push --set-upstream origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 773 bytes | 26.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/jedidia-nku/Gym-Git-Exercise-Solution/pull/new/ft/contact-page
remote:
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
Revert "feat: add team page"
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "feat: add a faq page"
[ft/faq-page 5ded994] feat: add a faq page
 create mode 100644 faq.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 476 bytes | 34.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/jedidia-nku/Gym-Git-Exercise-Solution/pull/new/ft/faq-page
remote:
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/faq-page -> ft/faq-page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git revert b6eb2b113205aa263e9b9ecd67a0cdfd3b0e73d0 
[ft/faq-page 3e6ac5f] Revert "feat: add team page"
 1 file changed, 2 insertions(+), 2 deletions(-)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push --set-upstream origin ft/faq-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 400 bytes | 66.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
   5ded994..3e6ac5f  ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> 
```