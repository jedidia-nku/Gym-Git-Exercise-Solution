# GIT Exercise Solutions

## Bundle 1

### Exercise 1

```bush
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git init
Reinitialized existing Git repository in C:/Users/IT ZONE/OneDrive/Desktop/git-exercise/.git/
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "This is the first Exercise in the Bundle one"
On branch main
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git branch -M main
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git remote add origin https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git init
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add README.md
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git branch -M main
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> ^C
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git remote add origin https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
error: remote origin already exists.
Everything up-to-date
branch 'main' set up to track 'origin/main'.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout dev
error: pathspec 'dev' did not match any file(s) known to git
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git branch -D test
error: branch 'test' not found.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b dev
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
 * [new branch]      dev -> dev
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git checkout dev
Switched to branch 'dev'
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git branch -D test
Deleted branch test (was 26a223a).
```

### Exercise 2

```bush
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git status
Untracked files:

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add home.html
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add about.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on dev: 26a223a This is the exercise one of bundle one
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html
Saved working directory and index state WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop^C
error: unknown switch `e'
usage: git stash pop [--index] [-q | --quiet] [<stash>]

    --index               attempt to recreate the index

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
error: unknown switch `e'
usage: git stash pop [--index] [-q | --quiet] [<stash>]
    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
error: unknown switch `e'

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> ^C
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{3}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> ^C
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop stash@{2}
error: unknown switch `e'
usage: git stash pop [--index] [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> ^C
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)

Dropped refs/stash@{0} (ab86f2b29e19ce8b40579c848d80afe356574129)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop
Auto-merging team.html
CONFLICT (add/add): Merge conflict in team.html
On branch dev
  (use "git add <file>..." to mark resolution)
        both added:      team.html
no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop stash@{1}
error: unknown switch `e'
usage: git stash pop [--index] [-q | --quiet] [<stash>]
    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{3}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git pop stash@{2}
The most similar command is
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop stash@{2}
error: unknown switch `e'
usage: git stash pop [--index] [-q | --quiet] [<stash>]

    --index               attempt to recreate the index

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html
Dropped refs/stash@{0} (9607f6e8b2289a2320f55d7015a581d16ad5cfbe)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{3}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash apply stash@{0}
error: unknown switch `e'
usage: git stash apply [--index] [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> ^C
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop 'stash@{2}:'
fatal: 'stash@{2}:' is not a stash-like commit
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{3}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash 'stash@{2}'
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'stash@{2}'
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop 'stash@{2}'
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)

Dropped stash@{2} (5c17cfbf946fd62c43a8dec28dac98d7a15cc68d)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop 'stash@{2}'
On branch dev
        new file:   about.html
        new file:   home.html

Dropped stash@{2} (ba4b3568b37334d5bbb8c26dcf3e737689832280)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{1}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash pop 'stash@{1}'
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html
Dropped stash@{1} (05da20cdd9d09d17b55188064fc728bd5a544f3d)
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add --all
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git commit -m "set up the home and about page"
[dev 8774772] set up the home and about page
 3 files changed, 36 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push
fatal: The current branch dev has no upstream branch.

To have this happen automatically for branches without a tracking
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git push --set-upstream origin dev
Counting objects: 100% (6/6), done.
Writing objects: 100% (5/5), 648 bytes | 58.00 KiB/s, done.
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/jedidia-nku/Gym-Git-Exercise-Solution.git
   26a223a..8774772  dev -> dev
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
No local changes to save
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html  
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on dev: 8774772 set up the home and about page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team
fatal: pathspec 'team' did not match any files
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git add team.html
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash
Saved working directory and index state WIP on dev: 8774772 set up the home and about page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git stash list
stash@{0}: WIP on dev: 8774772 set up the home and about page
stash@{1}: WIP on dev: 8774772 set up the home and about page
stash@{2}: WIP on dev: 26a223a This is the exercise one of bundle one
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git reset --hard
HEAD is now at 8774772 set up the home and about page
PS C:\Users\IT ZONE\OneDrive\Desktop\git-exercise> git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
````