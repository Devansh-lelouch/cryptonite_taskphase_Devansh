# Comprehending Commands
 The Third module ( I have to complete this by tonight becuase i was "quencing my thirst" and failed at it )

## Cat:Not the pet but the command

cat command is used for reading files 
We directly read a file called flag to  get the flag using `cat flag`
The flag is :
>pwn.college{I3YL_-3fN_LgmxMmvBCxmXcLKMG.dFzN1QDL4YjN0czW}

## Catting absolute paths 
Use cat command to read a file through its directory using `cat /flag`
The flag is :
>pwn.college{wWXi3eY-7GCjoepfqdg9F1WhhHv.dlTM5QDL4YjN0czW}

## More catting pratice 
Find the directory where flag is using `cd/flag` command. ( Says us to not use this but we get the directory using that only and not the find command )

use `cat` with the path you get to acces the flag 

The flag is:
>pwn.college{Uj61J7vwZFaJA7-EIu66hmaS17M.dBjM5QDL4YjN0czW}

## Grepping for needle in haysack

 Grep command is used to search for content in the files. 
 We have to search for the flag in a very large file called `/challenge/data.txt`
 Use `grep pwn.college /challenge/data.txt ` to get the flag as the flag starts with pwn.college

The flag is:
>pwn.college{MTz9rhyWW6Gb6z5zKqw_BlA06XH.ddTM4QDL4YjN0czW}

## Listing Files
ls command is use to list all the files and the directory a certain directory contains 

use `ls /challenge` to find the random file where the flag is stored 
The random file is `31781-renamed-run-2003`
Use ` /challenge/31781-renamed-run-2003`to get the flag 

The flag is :
>pwn.college{0SXt3hwZuo_9w8R5qo-PtK8buei.dhjM4QDL4YjN0czW}

## Touching Files
We touch  a file to create it ( HELLA SUS ) 
Use `touch /tmp/pwn` & `touch /tmp/college` to create files. 
The flag is : 
>pwn.college{wRfbr4Y2L7LeKPEbmyzvymjJV9x.dBzM4QDL4YjN0czW}

## Removing files 
We use rm to remove files.
Remove the file using `rm /delete_me` and then run the `/challenge/check`
The flag is:
>pwn.college{IurI3eQdSSObGCNyY-dvgn0owoq.dZTOwUDL4YjN0czW}

## Hidden Files
Sometimes ls wont display all the files as some files that start with `.` dont show up. In order to see those file you have to invoke ls with `-a`.
 
Change the directory to `/` and type in `ls -a` 
Use `cat` to read the hidden file and get the flag .
The flag is :
>pwn.college{M5_czuGwjsXY5HwB77S11RGplut.dBTN4QDL4YjN0czW}

## An Epic filesystem Quest
 In this challenge we have to play a small clue based game to find the flag

1 . `cd` to /

2.  `ls` all the files 

3 . Read the clue file 

4. `ls` the clue file and then read that file to get next hint 

Keep doing this till you get the flag 
>pwn.college{IjnpkW_-JJw0DpC7CyUZ-qsiYFi.dljM4QDL4YjN0czW}

## Making Directories
You make directories using the mkdir command.
make a directory using `mkdir/tmp/pwn`and use the `touch college` to create a file called college within it 

The Flag is :
>pwn.college{Y7tFiHpu3QOpPhbNRFSotN4KTAn.dFzM4QDL4YjN0czW}

## Finding Files
use command find to `find` directories.
```
find / -name flag
find: ‘/root’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
find: ‘/tmp/tmp.G9qthVCks5’: Permission denied
/usr/local/share/radare2/5.9.5/flag
/usr/local/lib/python3.8/dist-packages/pwnlib/flag
find: ‘/var/cache/apt/archives/partial’: Permission denied
find: ‘/var/cache/ldconfig’: Permission denied
find: ‘/var/cache/private’: Permission denied
find: ‘/var/log/private’: Permission denied
find: ‘/var/log/apache2’: Permission denied
find: ‘/var/log/mysql’: Permission denied
find: ‘/var/lib/apt/lists/partial’: Permission denied
find: ‘/var/lib/mysql-keyring’: Permission denied
find: ‘/var/lib/php/sessions’: Permission denied
find: ‘/var/lib/private’: Permission denied
find: ‘/var/lib/mysql-files’: Permission denied
find: ‘/var/lib/mysql’: Permission denied
find: ‘/run/mysqld’: Permission denied
find: ‘/run/sudo’: Permission denied
find: ‘/proc/tty/driver’: Permission denied
find: ‘/proc/1/task/1/fd’: Permission denied
find: ‘/proc/1/task/1/fdinfo’: Permission denied
find: ‘/proc/1/task/1/ns’: Permission denied
find: ‘/proc/1/fd’: Permission denied
find: ‘/proc/1/map_files’: Permission denied
find: ‘/proc/1/fdinfo’: Permission denied
find: ‘/proc/1/ns’: Permission denied
find: ‘/proc/7/task/7/fd’: Permission denied
find: ‘/proc/7/task/7/fdinfo’: Permission denied
find: ‘/proc/7/task/7/ns’: Permission denied
find: ‘/proc/7/fd’: Permission denied
find: ‘/proc/7/map_files’: Permission denied
find: ‘/proc/7/fdinfo’: Permission denied
find: ‘/proc/7/ns’: Permission denied
/opt/linux/linux-5.4/drivers/pnp/pnpbios/flag
/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
/opt/radare2/libr/flag
/nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag
/nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag
```
Use `cat /opt/linux/linux-5.4/drivers/pnp/pnpbios/flag` to get the flag.


## Linking Files 
In this challenge, we will learn about symbolic links (also also known as symlinks). Symbolic links are created with the ln command with the -s argument


we have to read ` /home/hacker/not-the-flag ` file by making the file `flag` point towards it so we use the command
`ln -s /flag /home/hacker/not-the-flag` to do this . 
Now we run the `challenge/catflag` to get the flag. 

The Flag is : 
>pwn.college{Qrt3b-vSGEQ55CEJx6lgaKbg_KJ.dlTM1UDL4YjN0czW}

