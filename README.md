# GitCLI_Test
This explains the basic commands needed in using Git CLI. Windows Commands :)

Git Download Links
-Linux (Debian): $ sudo apt-get install git
-Linux (Fedora): $ sudo yum install git
-Mac: http://git-scm.com/download/mac
-Window: http://git-scm.com/download/win

Git Commands
- $ touch <file>		              //Creating a file. Add filename and filetype
- $ git init 			                //Initiaize local git repository
-          //To configure your git account
	- $ git config --global user.name '<Your GitHub Username>'
	- $ git config --global user.email '<Your GitHub Email>'
- $ git add <file> 		            //Add file(s) to index
- $ $ git rm --cached <file>			//Removes files from index	
- $ git status			              //Check status of working tree
- $ git commit			              //Commit changes in index
	click on I. Then enter comment text. click on 'ESC'. Then type ':wq' and hit enter.
	OR    - $ git commit -m '<comment here>' {RECOMMENDED}.	
- $ git push			                //Push to remote repository
- $ git pull			                //Pull latest from remote repository
- $ git clone			                //Clone repository into a new directory 
- $ git branch <branch_name>			//Creates a new Branch
- $ git checkout		              //Swithches Branch
- $ git merge			                //To merge branches
- $ git remote			              //To list the remote repository available

Useful Keys
- *.<filetype>			              //Adds every file with that filetype
- .						                    //Adds everything in that folder


------Example

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code
$ touch app.js

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code
$ git init
Initialized empty Git repository in C:/Users/<Your computer username>/Documents/Test VS Code/.git/

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git config --global user.name '<Your GitHub Username>'

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git config --global user.email '<Your GitHub Email>'

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git add index.html

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.js
        style.css


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git rm --cached index.html
rm 'index.html'

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.js
        index.html
        style.css

nothing added to commit but untracked files present (use "git add" to track)

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git add *.html

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.js
        style.css


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git rm --cached index.html
rm 'index.html'

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.js
        index.html
        style.css

nothing added to commit but untracked files present (use "git add" to track)

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git add .

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js
        new file:   index.html
        new file:   style.css


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js
        new file:   index.html
        new file:   style.css

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   app.js


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git add .

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js
        new file:   index.html
        new file:   style.css


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git commit
[master (root-commit) 3058e65] Initial Commit
 3 files changed, 21 insertions(+)
 create mode 100644 app.js
 create mode 100644 index.html
 create mode 100644 style.css

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master
nothing to commit, working tree clean

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   app.js

no changes added to commit (use "git add" and/or "git commit -a")

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git add .

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git commit -m 'Edited app.js'
[master aed4948] Edited app.js
 1 file changed, 1 insertion(+), 1 deletion(-)

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ clear

------DONE!!!




Git Ignore
- $ touch .gitignore

-------Example

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ touch .gitignore

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ touch log.txt

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git add .

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git add .

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   dir2/app.js


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ clear

------DONE!!!!




Branches and Merge branches

---------Example
<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git branch Login

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   dir2/app.js


<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git commit -m 'Edited for Git Ignore'
[master eb751a6] Edited for Git Ignore
 2 files changed, 3 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 dir2/app.js

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git checkout Login
Switched to branch 'Login'

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (Login)
$ touch login.html

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (Login)
$ git add .

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (Login)
$ git commit -m 'Edited for login'
[Login 7408dfa] Edited for login
 4 files changed, 5 insertions(+)
 create mode 100644 dir1/app.js
 create mode 100644 log.txt
 create mode 100644 login.html

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (Login)
$ git checkout master
Switched to branch 'master'

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ git merge login
Merge made by the 'recursive' strategy.
 dir1/app.js | 1 +
 index.html  | 2 ++
 log.txt     | 1 +
 login.html  | 1 +
 4 files changed, 5 insertions(+)
 create mode 100644 dir1/app.js
 create mode 100644 log.txt
 create mode 100644 login.html

<Your computer username>@DESKTOP-8FI3LUO MINGW64 ~/Documents/Test VS Code (master)
$ clear

-----------DONE!!!




Remote Repository

-Create a repository online on GitHub
- $ git remote
- $ git remote add origin <GitHub Repository Link>
- $ git remote
- $ git push -u origin master

PS: Remeber to create a README.md file.
 



Clone a Repository

- $ git clone <repository_link>			//To download a repository
