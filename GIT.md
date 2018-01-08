# What is Markdown?

## Overview

Markdown is comparable to HTML in that you can define the pages formatting through text based commands. The advantage however is the simplicity meaning that people with little training can create webpages, notes and emails using a lightweight and intuitive form.

##Key Syntax Rules

To determine headlines a hashtag is placed before the text and the number of sequential hashtags determines how small the font is. 

#Main-Header

##Sub-Header

###And so on...

Furthermore including image links is simply done by referencing the online copy after ![Caption](ImageLink]

![Example Ubuntu Image](https://tr2.cbsistatic.com/hub/i/r/2016/08/09/e450825d-6592-49cd-a2a8-e172ef086841/resize/770x/d43e6e8ffe1465f20fe473f7d58cc896/ubuntuhero.jpg)

To include local files they must be added to the github repo. and then linked using the webpage address.


Bullet points are created using a dash like so:

- Example Uno

To make pieces of text **BOLD** two astrisks are placed either side of the text. *Italics* however are made only using the one astrisk.

To include sections of code three grove accents are placed either side of the extractt

```
Like so
```


Finally all documents are stored in the .md format to ensure correct formatting when opened.



# Command Line 101

# Breakdown of linux commands

- ls
 
Prints the directory list of the home path route

```
othom@othom-Alienware-15-R2:~$ ls
Arduino    examples.desktop      Pictures               ROSSTL
Desktop    First Task - ROCO222  Public                 sketchbook
Dev        hello-hello.md        robot-arm-custom.urdf  src
Documents  Journal-General.md    robot-project          Templates
Downloads  Music                 ROCO222                Videos
```

- cd /tmp

Specifies the 'Current Directory' as route /tmp. This allows you to create/ modify files in that file location.

- cd $HOME

Specifies the 'Current Directory' as /home. The '$' sign asks linux to insert any variation of the home address specific to the workstation and therefore is a more generalised command.

- mkdir

Stands for 'Make Directory' and allows for you to create a folder/ directory as an extension as the one you're currently in.

- echo "Hello" > hello.md

Creates a file named 'hello.md' and populates it with the text 'Hello'. The 'echo' command outputs the inputted string as an argument. 

- cat hello.md

Reads and displays the contents of the file 'hello.md'. The command 'cat' is short for concatenate and is used to view of obtain files in a terminal. 

- cp hello.md hello-again.md

cp copies the contents of the file 'hello.md' into a new file called 'hello-again.md'

- mv hello-again hello-hello.md

Moves hello-again.md into the directory of hello-hello.md

- rm hello.md

Removes the file hello.md

- rm -rf

A dangerous command comprised of two sections. The r is a recursive remove and the f forces the action. For example

```
rm -rf ~
```

Would remove all your files - Recursively and with force (Root access)


- cat/proc/cpuinfo

recalls and prints the contents of file cpuinfo into the terminal


# Copy of the terminal after all commands

```

othom@othom-Alienware-15-R2:~$ ls
Desktop    Downloads         First Task - ROCO222  Music     Public   Templates
Documents  examples.desktop  hello-hello.md        Pictures  ROCO222  Videos
othom@othom-Alienware-15-R2:~$ cd /tmp
othom@othom-Alienware-15-R2:/tmp$ cd $HOME
othom@othom-Alienware-15-R2:~$ mkdir Test
othom@othom-Alienware-15-R2:~$ echo "Hello" > hello.md
othom@othom-Alienware-15-R2:~$ cat hello.md
Hello
othom@othom-Alienware-15-R2:~$ cp hello.md hello-again.md
othom@othom-Alienware-15-R2:~$ mv hello-again.md hello-hello.md
othom@othom-Alienware-15-R2:~$ rm hello.md
othom@othom-Alienware-15-R2:~$ rm -rf
othom@othom-Alienware-15-R2:~$ cat /proc/cpuinfo
processor	: 0
vendor_id	: GenuineIntel
cpu family	: 6
model		: 94
model name	: Intel(R) Core(TM) i7-6700HQ CPU @ 2.60GHz
stepping	: 3
microcode	: 0x84
cpu MHz		: 1571.362
cache size	: 6144 KB

[Terminal continues to print the rest of cpuinfo file]


```







## Your First Repo

## Git Repository and Hidden Files - Taking it further

"Type ls -al and describe the different informations displayed"

```
othom@othom-Alienware-15-R2:~/ROCO222/Ollie/Journal$ ls -al
total 40
drwxrwxr-x 3 othom othom 4096 Sep 30 14:33 .
drwxrwxr-x 3 othom othom 4096 Sep 28 19:46 ..
drwxrwxr-x 8 othom othom 4096 Sep 30 14:30 .git
-rw-rw-r-- 1 othom othom 1971 Sep 30 14:32 Journal-Command101.md
-rw-rw-r-- 1 othom othom  997 Sep 30 14:32 Journal+Command101.md
-rw-rw-r-- 1 othom othom    0 Sep 30 14:32 Journal-GitRepo.md
-rw-rw-r-- 1 othom othom  729 Sep 28 20:34 Journal-GoingSocial.md
-rw-rw-r-- 1 othom othom  927 Sep 30 14:33 Journal.md
-rw-rw-r-- 1 othom othom   24 Sep 28 20:40 Journal-SSH.md
-rw-rw-r-- 1 othom othom  190 Sep 28 20:02 Journal_v1.0.md
-rw-rw-r-- 1 othom othom  521 Sep 28 20:02 README.md
othom@othom-Alienware-15-R2:~/ROCO222/Ollie/Journal$ 
```

- "drwxrwxr-x 3 othom othom 4096 Sep 30 14:33 ."

This refers to a hidden tempory file within the repo.

- "-rw-rw-r-- 1 othom othom 1971 Sep 30 14:32 Journal-Command101.md"

This is a working document stored within the location which can be readily read and written to.

# Breaking down the given information

- "drwxrwxr-x" & "-rw-rw-r--"

drwxrwxr-x means that .git is a directory. When entered the following files are within:

```
drwxrwxr-x  8 othom othom 4096 Sep 30 14:30 .
drwxrwxr-x  3 othom othom 4096 Sep 30 14:42 ..
drwxrwxr-x  2 othom othom 4096 Sep 28 20:01 branches
-rw-rw-r--  1 othom othom  360 Sep 30 14:30 COMMIT_EDITMSG
-rw-rw-r--  1 othom othom  337 Sep 30 13:42 config
-rw-rw-r--  1 othom othom   73 Sep 28 20:01 description
-rw-rw-r--  1 othom othom   81 Sep 28 20:02 FETCH_HEAD
-rw-rw-r--  1 othom othom  377 Sep 30 13:43 gitk.cache
-rw-rw-r--  1 othom othom   23 Sep 28 20:01 HEAD
drwxrwxr-x  2 othom othom 4096 Sep 28 20:01 hooks
-rw-rw-r--  1 othom othom  473 Sep 30 14:30 index
drwxrwxr-x  2 othom othom 4096 Sep 28 20:01 info
drwxrwxr-x  3 othom othom 4096 Sep 28 20:02 logs
drwxrwxr-x 39 othom othom 4096 Sep 30 14:30 objects
drwxrwxr-x  5 othom othom 4096 Sep 28 20:05 refs
```

-rw-rw-r-- files with this code are readable and writable documents.


- "3,3,8,1,..."

These values co-respond to the number of files held within the named directory/ files. The top three directories therefore all have values greater than 1 as they contain multiple files.

- "othom"

Co-responds to the username of the file owner

- "4096, 4096, 4096, 1971"

Refers to the size of each file with units of bytes.

- Time

A date and time stamp are placed afterwards 

- File Names

These are put at the end of the line.


## First Commit

To upload files to the git server a commit is ran. This not only stores/ updates the server but allows your to add a descriptive comment allowing for good version tracking and collaborative working.

```
git commit
```

Brings you to 

```


# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
# On branch master
# Your branch is up-to-date with 'origin/master'.
#
# Changes to be committed:
#       new file:   Example.md
#
# Changes not staged for commit:
#       modified:   Journal-General.md
#       modified:   Journal-Hacking.md
#






                               [ Read 13 lines ]
^G Get Help  ^O Write Out ^W Where Is  ^K Cut Text  ^J Justify   ^C Cur Pos
^X Exit      ^R Read File ^\ Replace   ^U Uncut Text^T To Spell  ^_ Go To Line

```

A comment is placed at the top and the document is stored.



## Version Tracking

Running the 'git status' command will present the documents which have been altered but not yet uploaded to the remote git repo. 

I've just committed all my working files but linux is aware of two files that have never been uploaded and therfore isn't tracking

```
othom@othom-Alienware-15-R2:~/ROCO222/Ollie/Journal$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	Journal-SSH.md
	Journal-VersionTracking.md

nothing added to commit but untracked files present (use "git add" to track)
```

When 'Journal-VersionTracking.md' is added git will start tracking the document. 

```
othom@othom-Alienware-15-R2:~/ROCO222/Ollie/Journal$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   Journal-VersionTracking.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	Journal-SSH.md
```

Under 'changes' the file is shown with the tracking enabled.

When commited the version updated with commit comments will be recorded.



# Going Social

## Push

In order to upload and download files from the Github rep. a push/ pull command is used in the terminal. 

To do this follow the steps below:

Ensure your current directory is the same as the file's location.

Add the online repository by using the 'git remote add origin /Link to github repo'

This will now define where to send the files onced pushed. 

Pushing the entire contents of the local directory into the remote repo is achieved by using the following command. 

'git push -u origin' Where 'origin' is a user defined name for the remote

## Pull

Similarly should you want to pull/download from the github repo the following command is used 

'git pull' 

This will download the entire repo. 




#Generating SSH Codes

After the SSH key has been generated it can be added to the SSH agent. The SSH information is kept in the following file 

```
-rw-r--r--  1 othom othom  767 Sep 28 20:57 id_rsa.pub
```

The SSH private key is then added to the SSH agent.

```
othom@othom-Alienware-15-R2:~$ ssh-add ~/.ssh/id_rsa
Enter passphrase for /home/othom/.ssh/id_rsa: 
Identity added: /home/othom/.ssh/id_rsa (/home/othom/.ssh/id_rsa)
```

Estabilishing a connection with Github is done as follows

```
othom@othom-Alienware-15-R2:~$ ssh -T git@github.com
Hi OThom17! You've successfully authenticated, but GitHub does not provide shell access.
othom@othom-Alienware-15-R2:~$ 
```

Because up until now I've used a https link to push and not SSH the repo. will need to be cloned for SSH.

```
othom@othom-Alienware-15-R2:~$ git clone git@github.com:OThom17/Lab-Journal.git
Cloning into 'Lab-Journal'...
remote: Counting objects: 51, done.
remote: Compressing objects: 100% (40/40), done.
remote: Total 51 (delta 22), reused 37 (delta 10), pack-reused 0
Receiving objects: 100% (51/51), 8.52 KiB | 0 bytes/s, done.
Resolving deltas: 100% (22/22), done.
Checking connectivity... done.
othom@othom-Alienware-15-R2:~$ 
```




















