Aqui está todas execuções que realizei no bash:


user@usuariopc MINGW64 ~/Documents/_git/entrega-git
$ git init
Initialized empty Git repository in C:/Users/user/Documents/_git/entrega-git/.gi
t/

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (master)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (master)
$ git add README.md

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.txt


user@usuariopc MINGW64 ~/Documents/_git/entrega-git (master)
$ git add .

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (master)
$ git commit -m "Salvando alterações do readme e index"
[master (root-commit) f501867] Salvando alterações do readme e index
 2 files changed, 6 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.txt

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (master)
$ git branch -m main

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git remote add origin https://github.com/todyzera/entrega-git.git

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 361 bytes | 361.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/todyzera/entrega-git.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git checkout
Your branch is up to date with 'origin/main'.

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git branch feature1

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git checkout feature1
Switched to branch 'feature1'

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ ls
README.md  index.txt

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git commit "Criação da branch feature1"
error: pathspec 'Criação da branch feature1' did not match any file(s) known to
git

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git commit -m "Criação da branch feature1"
On branch feature1
nothing to commit, working tree clean

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git push -u origin main
branch 'main' set up to track 'origin/main'.
Everything up-to-date

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git checkout feature1
M       index.txt
Switched to branch 'feature1'

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git commit -m "alteração no index"
On branch feature1
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.txt

no changes added to commit (use "git add" and/or "git commit -a")

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git add .

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git commit -m "alteração no index"
[feature1 3a05d54] alteração no index
 1 file changed, 1 insertion(+), 1 deletion(-)

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (feature1)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git merge feature1
Updating f501867..3a05d54
Fast-forward
 index.txt | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ ^C

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 365 bytes | 365.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/todyzera/entrega-git.git
   f501867..3a05d54  main -> main

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git push origin feature1
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'feature1' on GitHub by visiting:
remote:      https://github.com/todyzera/entrega-git/pull/new/feature1
remote:
To https://github.com/todyzera/entrega-git.git
 * [new branch]      feature1 -> feature1

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git add .

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git push origin main
Everything up-to-date

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.txt


user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git commit -m "alteração no index de main"
[main 19a2cb8] alteração no index de main
 1 file changed, 1 insertion(+), 1 deletion(-)

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 368 bytes | 368.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/todyzera/entrega-git.git
   3a05d54..19a2cb8  main -> main

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$ git merge feature1
Already up to date.

user@usuariopc MINGW64 ~/Documents/_git/entrega-git (main)
$
