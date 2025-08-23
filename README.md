USE@DESKTOP-P4J51PO MINGW64 ~
$ git clone git@github.com:siddu1995-web/decsecoppatil
Cloning into 'decsecoppatil'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

USE@DESKTOP-P4J51PO MINGW64 ~
$ cd decsecoppatil

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil (main)
$ mkdir 2025-08-04

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil (main)
$ cd 2025-08-04

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ touch task1 task2

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ./

nothing added to commit but untracked files present (use "git add" to track)

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git add .

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   task1
        new file:   task2


USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git commit -m "Intial commit with two task files"
[main ff3d6f0] Intial commit with two task files
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 2025-08-04/task1
 create mode 100644 2025-08-04/task2

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ echo "This is task1" >>task1

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   task1

no changes added to commit (use "git add" and/or "git commit -a")

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git add .
warning: in the working copy of '2025-08-04/task1', LF will be replaced by CRLF the next time Git touches it

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git commit "Updated task1 with the content"
error: pathspec 'Updated task1 with the content' did not match any file(s) known to git

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git log
commit ff3d6f0120846b51cc5668765fcd7c39de4c385a (HEAD -> main)
Author: siddu <siddanagouda6820@gmail.com>
Date:   Sat Aug 23 10:41:27 2025 +0530

    Intial commit with two task files

commit 8eae9fbe803e4f16da73923870a204b16d3b165b (origin/main, origin/HEAD)
Author: siddu1995-web <siddanagouda6820@gmail.com>
Date:   Sat Aug 23 10:34:17 2025 +0530

    Initial commit

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git show ff3d6f0120846b51cc5668765fcd7c39de4c385a
commit ff3d6f0120846b51cc5668765fcd7c39de4c385a (HEAD -> main)
Author: siddu <siddanagouda6820@gmail.com>
Date:   Sat Aug 23 10:41:27 2025 +0530

    Intial commit with two task files

diff --git a/2025-08-04/task1 b/2025-08-04/task1
new file mode 100644
index 0000000..e69de29
diff --git a/2025-08-04/task2 b/2025-08-04/task2
new file mode 100644
index 0000000..e69de29

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 345 bytes | 57.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:siddu1995-web/decsecoppatil
   8eae9fb..ff3d6f0  main -> main

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ echo "This is content of task2" >>task2

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   task1

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   task2


USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git add .
warning: in the working copy of '2025-08-04/task2', LF will be replaced by CRLF the next time Git touches it

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git commit -m "Updated content task2"
[main 4a81146] Updated content task2
 2 files changed, 2 insertions(+)

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 401 bytes | 100.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:siddu1995-web/decsecoppatil
   ff3d6f0..4a81146  main -> main

USE@DESKTOP-P4J51PO MINGW64 ~/decsecoppatil/2025-08-04 (main)
$
# decsecoppatil
