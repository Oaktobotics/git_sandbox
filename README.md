# git_sandbox
A git test sandbox for becoming familiar with version control

This guide is meant to help get you started using git as well as becoming familiar with the command linse and a few 
basic commands. Basic commands will have an explination 

---NOTE: iteration one will be targeted at unix like computers (Mac, linux, etc.) --

<b>What is git?</b>
Git is a software version control software that will allow us to edit and store the same code files in a decentralized
location. This will save having to send file to every team member and allow us to track all changes made to our code.
A detailed explination about git can be found here: https://git-scm.com/book/en/v2/Getting-Started-Git-Basics

<b>Step 0:</b> Getting Git
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





