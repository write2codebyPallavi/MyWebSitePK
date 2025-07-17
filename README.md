# repo
Git command
1. $ cd desktop
2. $ cd flodername
3. $ git config --global user.name "namw"
4. path$ git config --global user.email "qbc@gmail.com"
5. $ git config --list
6. $ git init
Initialized empty Git repository in C:/Users/ xxx/Desktop/ xxxwork/.git/

 
$ ls -la
total 32
drwxr-xr-x 1  xxx 197121    0 Jul 17 14:44 ./
drwxr-xr-x 1  xxx 197121    0 Jul 17 14:40 ../
drwxr-xr-x 1  xxx 197121    0 Jul 17 14:44 .git/
-rw-r--r-- 1  xxx 197121 2989 Jul 17 13:31 HomePage.html
-rw-r--r-- 1  xxx 197121 2188 Jul 17 14:02 table.html

 
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        HomePage.html
        table.html

nothing added to commit but untracked files present (use "git add" to track)

 
$ git add HomePage.html

 
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   HomePage.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        table.html


 
$ git commit -m "First v1 of HomePage.html"
[master (root-commit) 3d12435] First v1 of HomePage.html
 1 file changed, 86 insertions(+)
 create mode 100644 HomePage.html

 
$ git log
commit  xxx125 (HEAD -> master)
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:48:11 2025 +0530

    First v1 of HomePage.html

 
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   HomePage.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        table.html

no changes added to commit (use "git add" and/or "git commit -a")

 
$ git diff
diff --git a/HomePage.html b/HomePage.html
index 700c105..568eedd 100644
--- a/HomePage.html
+++ b/HomePage.html
@@ -66,7 +66,7 @@
         <input type="Reset" value="Reset">
         <input type="Reset" value="Cancel">

-        <a href="C:/Users/ xxx/Desktop/Pallav work/table.html"> Go to table </a>
+        <a href="C:/Users/ xxx/Desktop/ xxxwork/table.html"> Go to table </a>

         <!--button onclick="window.location.href='table.html'">
              Go to table </button>-->

 
$ git add HomePage.html

 
$ git commit -m "2nd version"
[master 8bb25c2] 2nd version
 1 file changed, 1 insertion(+), 1 deletion(-)

 
$ git log
commit xxx59896 (HEAD -> master)
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:53:21 2025 +0530

    2nd version

commit  xxx125
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:48:11 2025 +0530

    First v1 of HomePage.html

 
$ git log
commit  xxx12559 (HEAD -> master)
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:55:00 2025 +0530

    Table commit

commit xxx59896
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:53:21 2025 +0530

    2nd version

commit  xxx125
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:48:11 2025 +0530

    First v1 of HomePage.html

 
$ git show  xxx125: HomePage.html
tree  xxx125:

HomePage.html

 
$ git checkout master --*
error: unknown option `*'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --[no-]guess          second guess 'git checkout <no-such-branch>' (default)
    --[no-]overlay        use overlay mode (default)
    -q, --[no-]quiet      suppress progress reporting
    --[no-]recurse-submodules[=<checkout>]
                          control recursive updating of submodules
    --[no-]progress       force progress reporting
    -m, --[no-]merge      perform a 3-way merge with the new branch
    --[no-]conflict <style>
                          conflict style (merge, diff3, or zdiff3)
    -d, --[no-]detach     detach HEAD at named commit
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -f, --[no-]force      force checkout (throw away local modifications)
    --[no-]orphan <new-branch>
                          new unborn branch
    --[no-]overwrite-ignore
                          update ignored files (default)
    --[no-]ignore-other-worktrees
                          do not check if another worktree is using this branch
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -p, --[no-]patch      select hunks interactively
    --[no-]ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


 
$ git status
On branch master
nothing to commit, working tree clean

 
$ git resore table.html
git: 'resore' is not a git command. See 'git --help'.

The most similar command is
        restore

 
$ git restore table.html

 
$ git add table.html

 
$ git status
On branch master
nothing to commit, working tree clean

 
$ git diff

 
$ git log
commit  xxx12559 (HEAD -> master)
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:55:00 2025 +0530

    Table commit

commit xxx59896
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:53:21 2025 +0530

    2nd version

commit  xxx125
Author:  xxx < xxx@gmail.com>
Date:   Thu Jul 17 14:48:11 2025 +0530

    First v1 of HomePage.html

 
$ git remote add orgin https://github.com/write2codeby xxx/repo

 
$ git branch -M main

path$ git push -u orgin main
remote: Permission to write2codeby xxx/repo.git denied to b701k.
fatal: unable to access 'https://github.com/write2codeby xxx/repo/': The requested URL returned error: 403

path$ cd desktop^C

path$ ^C

path$
