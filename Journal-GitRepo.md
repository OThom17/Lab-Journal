# Git Repository and Hidden Files

## "Type ls -al and describe the different informations displayed"

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
