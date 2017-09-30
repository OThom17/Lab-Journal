# Command Line 101

# Breakdown of linux commands

- ls
 
Prints the directory list of the home path route

- cd /tmp

Specifies the 'Current Directory' as route /tmp

- cd $HOME

Specifies the 'Current Directory' as /home. The '$' sign signifies a directory address

- mkdir

Stands for 'Make Directory'

- echo "Hello" > hello.md

Creates a file named 'hello.md' and populates it with the text 'Hello'. The 'echo' command outputs the inputted string as an argument. 

- cat hello.md

Reads and displays the contents of the file 'hello.md'. The command 'cat' is short for concatenate and us used to view of obtain files in a terminal. 

- cp hello.md hello-again.md

cp copies the contents of the file 'hello.md' into a new file called 'hello-again.md'

- mv hello-again hello-hello.md

Moves hello-again.md into the directory of hello-hello.md

- rm hello.md

Removes the file hello.md

- rm -rf

UNKNOWN

- cat/proc/cpuinfo

recalls and prints the contents of file cpuinfo into the terminal


# Copy of the terminal after all commands

"""

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


"""

