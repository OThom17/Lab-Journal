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




