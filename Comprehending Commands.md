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
