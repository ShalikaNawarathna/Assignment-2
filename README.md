# Assignment-2
Q2)
1-Create a repository named as “Assignment 2” in github with Readme.md file,
Questions must be paste in the readme file.

2-Clone your repository.
->
$ git clone  https://github.com/ShalikaNawarathna/Assignment-2.git
Cloning into 'Assignment-2'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

3- Add the text file that should have the answer of Q1.
->
 git add quiz1.txt

4-Add another file to do the following.
->
 touch anotherOne.txt

5-Create another branch
->
$ git checkout -b anotherBranch
Switched to a new branch 'anotherBranch'


6-Make changes to your files.
7-see if the file change is detected with git status.
->
$ git status
On branch anotherBranch

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   quiz1.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Assignment-2/
        anotherOne.txt


8-stage the changes with git add 
 ->
  $ git add .

9-  check that the add did what you expected with git status.
 ->
$ git status
On branch anotherBranch

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Assignment-2
        new file:   anotherOne.txt
        new file:   quiz1.txt

  
10-  make the commit with git commit.
11-Write a meaningful commit message (e.g. "Answers question 1")
 ->
  $ git commit -am "First question's answer"
[anotherBranch (root-commit) 0abcd36] First question's answer
 3 files changed, 3 insertions(+)
 create mode 160000 Assignment-2
 create mode 100644 anotherOne.txt
 create mode 100644 quiz1.txt


12- check that your working directory is clean with git status.
 ->
$ git status
On branch anotherBranch
nothing to commit, working tree clean

13- check that your commit succeeded as expected with git log
 ->
$ git log
commit 0abcd366d08a34bd7df4a888c4ea650fb576789b (HEAD -> anotherBranch)
Author: ShalikaNawarathna <shalikachathuranganii22@gmail.com>
Date:   Sun Sep 12 23:08:37 2021 +0530

    First question's answer

14-Push your code up to a github repository
 ->
$ git push origin anotherBranch
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 369 bytes | 369.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'anotherBranch' on GitHub by visiting:
remote:      https://github.com/ShalikaNawarathna/Assignment-2/pull/new/anotherBranch
remote:
To https://github.com/ShalikaNawarathna/Assignment-2.git
 * [new branch]      anotherBranch -> anotherBranch

