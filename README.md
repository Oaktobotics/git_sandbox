# git_sandbox
A git test sandbox for becoming familiar with version control

This guide is meant to help get you started using git as well as becoming familiar with the command linse and a few 
basic commands. Basic commands will have an explination 

---NOTE: iteration one will be targeted at unix like computers (Mac, linux, etc.) --

<b>What is git?</b>
Git is a software version control software that will allow us to edit and store the same code files in a decentralized
location. This will save having to send file to every team member and allow us to track all changes made to our code.
A detailed explination about git can be found here: https://git-scm.com/book/en/v2/Getting-Started-Git-Basics

<b>Step 0:</b> Getting Git<br />
Instrunctions for installing git on Linux and Mac
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

To test if you have git installed open up your terminal program and type the command `git --version` and hit enter.
The output should be something like "git version 2.4.9" 

<b>Step 1:</b> Getting this repository (Note this will not work if you do not have git installed)
This repository is located on github's server at the location "https://github.com/OaktonLunabotics/git_sandbox.git"

First we will want to make a folder on our computer that will hold this repository 
I like to put all my code in my home directory. Open up your terminal (if it is not already open).
To navigate to your home directory type `cd ~` <br />
  - Command explination<br />
    -- `cd` stands for change directory, meaning we want to move around in our computer's file system.<br />
    -- `~` on mac and most versions of linux the tilde stands fo your home directory.

Now that we are in our home directory let's make a file that will host our code.
Let's call it git_test. To do this type the command `mkdir ~/git_test` <br />
 - Command explination<br />
  -- `mkdir` stands for make drectory. The command is usually followed by the name of the directory we want to make

Our filder has been created so let's move to it with our change directory command: `cd git_test`
  <br />HINT: if you are no longer in the home directory you can use `cd ~/git_test`

Now we will grab the repository from github using the command 
`git clone https://github.com/OaktonLunabotics/git_sandbox.git` <br />
  <i>NOTE:</i> This may prompt you for your github username and password if you are not logged in.<br />

We have successfully copied the repository! To check that this has been done type the command `ls`. You should see
a new folder called 'git_sandox' (which is the name of our repository or file system stored on github).<br />
 - Command explination<br />
  -- `ls` simply stands for list. This will list everything in the current folder/directory you are in.

<b>Step 2:</b> Hello git! Your first commit. <br />
Let's make a change to this README. We will do so by adding our name to the bottom of the file. Don't worry if you accidetally delete the entire file, we can always get it back using an older version from github.

Change to the directory where the README is. Tt should be in our folder at "git_sandbox/READEME.md" so we will use the command `cd git_sandbox`.<br />
(If you follwed the steps above our full path will be: home->git_test->git_sandbox or ~/git_test/git_sandbox/)

now run the command `ls` and you should see our file `README.md`

-- Edit the file --<br />
Edit the file in your favorite text editor. Make sure you are editing the correct file in our repository path (path from above..~/git_test/git_sandbox/README.md) <br />
Add a greeting with your name to the bottom of the file like "Hello from \<your_name>"

Once the file has be edited pop back over to your terminal. Remember if you are not in the directory with our edited file, you can always change back with `cd ~/git_test/git_sandbox/`

Now that we are at our terminal in the correct directory type type `git status` <br /> 
 - What am I seeing? <br /> 
   -- you should see "modified:   README.md" in red this means that git is aware that you have made changes to this fie <br />
  -- The red color means that our file has been changed but not staged (i.e not ready to push to our remote github location)

We need to now stage (or <i>add</i>) our file. This means that we are getting ready to push and letteing git know that this file is ready to be merged into our github main branch. To stage (<i>add</i>) use the comand `git add <file_name>` in our case we will do `git add README.md` 

Now type `git status` again, our file should be green.

We are ready to commit!

Committing means that we are going to esentially stamp our code change with a unique ID so git can keep track of when it was changed. When you commit it is a good idea to add a helpful message briefly describing what changes you have made. <br />
To make a <i>commit</i> use the command `git commit -m "A descriptive message"`
 - What is this '-m' business?<br />
 -- '-m' is an argument to the git commit command. After all commit is a function from the program git.<br />
 -- after '-m' add a message in quotes and it will be attached with your commit and can be viewed by everone looking at the repository on github.

In my case I will do `git commit -m "added chris's greeting to the README"`

Now we have committed the file. If you run `git status` again you will notice that the modified file is no longer there.

The last thing we need to do is push our changes to github.

To <i>push</i> our code up the command is simply `git push`










