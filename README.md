# Assignment10--CISC3140

### Objective: Set up an automated deployment strategy. This sounds more complicated than it really is, which is creating a a yaml file for your app from the previous assignment in the format specified by your tool of choice. The ultimate goal is to deploy your app to a server somewhere, such as Google App Engine (GAE), Heroku, etc.

#### Hiude-MacBook-Pro:~ hiuwing.l$ git init
    Initialized empty Git repository in /Users/hiuwing.l/.git/
    
#### Hiude-MacBook-Pro:~ hiuwing.l$ git remote add origin git@github.com:hiuwing0107/Assignment10--CISC3140.git

#### Hiude-MacBook-Pro:~ hiuwing.l$ git status
    On branch master

    No commits yet

    Untracked files:
     (use "git add <file>..." to include in what will be committed)
     
  	Assignment10--CISC3140/

    nothing added to commit but untracked files present (use "git add" to track)
    
#### Hiude-MacBook-Pro:~ hiuwing.l$ cd Assignment10--CISC3140/

#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git status
    On branch master
    Your branch is up to date with 'origin/master'.

    nothing to commit, working tree clean
    
#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git log
    commit 2a3451a45de79c5b993b99dc0ad69b7566b569bc (HEAD -> master, origin/master, origin/HEAD)
    Author: hiuwing0107 <42844009+hiuwing0107@users.noreply.github.com>
    Date:   Fri Apr 17 21:35:37 2020 -0400

         Initial commit
         
#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git checkout -b travis
    Switched to a new branch 'travis'
    
#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ vim .travis.yml

#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git status
    On branch travis
    Untracked files:
      (use "git add <file>..." to include in what will be committed)

    	.travis.yml

    nothing added to commit but untracked files present (use "git add" to track)
    
#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git add .

#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git status
    On branch travis
    Changes to be committed:
      (use "git reset HEAD <file>..." to unstage)

    	new file:   .travis.yml

#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git commit -m"Added Travis File"
    [travis 0ca2b5a] Added Travis File
     Committer: Hiu Wing Lam <hiuwing.l@Hiude-MacBook-Pro.local>
    Your name and email address were configured automatically based
    on your username and hostname. Please check that they are accurate.
    You can suppress this message by setting them explicitly:

        git config --global user.name "Your Name"
        git config --global user.email you@example.com

    After doing this, you may fix the identity used for this commit with:

        git commit --amend --reset-author

     1 file changed, 6 insertions(+)
     create mode 100644 .travis.yml
     
#### Hiude-MacBook-Pro:Assignment10--CISC3140 hiuwing.l$ git push origin travis
    Enumerating objects: 6, done.
    Counting objects: 100% (6/6), done.
    Delta compression using up to 8 threads
    Compressing objects: 100% (4/4), done.
    Writing objects: 100% (6/6), 949 bytes | 949.00 KiB/s, done.
    Total 6 (delta 0), reused 0 (delta 0)
    remote: 
    remote: Create a pull request for 'travis' on GitHub by visiting:
    remote:      https://github.com/hiuwing0107/Assignment10--CISC3140/pull/new/travis
    remote: 
    To https://github.com/hiuwing0107/Assignment10--CISC3140.git
     * [new branch]      travis -> travis

----------------------------------------------------------------------------------------------------------------------------
CISC 3140 - Design and Implementation

Professor: Katherine Chuang

Student Name: Hiu Wing, Lam

Emplid: 23626630

Assignment 10 - Continuous Integration
