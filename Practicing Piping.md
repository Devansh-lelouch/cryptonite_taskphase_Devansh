# Practicing Piping
Sixth module talking about input output redirection

## Redirecting Output
`>`character is used  to give output in a file 
`echo PWN > COLLEGE` will write PWN in the file COLLEGE
The Flag is :
>pwn.college{A2HQbH1sN1AwJg3mbm_gWqrtq07.dRjN1QDL4YjN0czW}

 ## Redirecting More output
We can redirect commands to a output as well 
`/challenge/run > myflag` will redirect the output of `/challenge/run ` to myflag
printing myflag with `cat myflag` will get you the output (i.e flag ) from `/challenge/run` 

The Flag is 
>pwn.college{4L-jlg03htA5doWdpYXhj7Ur9ES.dVjN1QDL4YjN0czW}

## Appending Output
We use `>>` to append data into the file as using `>` just overwites the data in the file 
 `/challenge/run >> /home/hacker/the-flag` to get the flag 
The flag is : 
>pwn.college{Ict2abvP-GTO3qHG5pH3dTiQ2UJ.ddDM5QDL4YjN0czW}

## Redirecting Errors
FD 0: Standard Input
FD 1: Standard Output
FD 2: Standard Error 
where FD refers to File Descriptions 

`/challenge/run > myflag 2> instructions` where 2 referes to FD2 

The Flag is : 
 >pwn.college{wL5VgQwDf5-pLna0jbxYqkdlfcm.ddjN1QDL4YjN0czW}

## Redirecting Inputs 
Use 

```
echo COLLEGE > PWN
```
to redirect the output of echo COLLEGE to PWN

Use` /challenge/run < PWN `to redirect the file PWN as input to /challenge/run


The Flag is :
>pwn.college{YemPgxTAEQzlGMXfKKO4hQn9nt3.dBzN1QDL4YjN0czW}

## Grepping Stored results 
Redirect the output of  of `/challenge/run` to `/tmp/data.txt` using
Grep the file as the name starts from `pwn.college` using `grep pwn.college /tmp/data.txt`


The flag is :
>pwn.college{AkWA5fjtbOesHNSFCeWZCj5PDPS.dhTM4QDL4YjN0czW}

## Grepping live output

pipe | command can be used to avoide stroing results into a file 

`/challenge/run | grep pwn.college` connect `/challenge/run` to `grep pwn.college` by using `|`

The Flag is :
>pwn.college{IlffW83-4cMKZktdTtUDkr_cwul.dlTM4QDL4YjN0czW}

## Grepping errors
The > operator redirects a given file descriptor to a file, and you've used 2> to redirect fd 2, which is standard error. The | 
operator redirects only standard output to another program, and there is no 2| form of the operator! It can only redirect standard 
output (file descriptor 1)

The shell has a >& operator, which redirects a file descriptor to another file descriptor. This means that we can have a two-step
process to grep through errors: first, we redirect standard error to standard output (2>& 1) and then pipe the now-combined stderr
and stdout as normal (|)!

>pwn.college{AVdM5iWv7aiYsZVavyEh6HNfREQ.dVDM5QDL4YjN0czW}

## Duplicating piped data with tee
`/challenge/pwn | tee doracake | /challenge/college`  Intercepts the command by using tee.
`cat` into `doracake`
We get the secret  argument to run the command and get the flag with 
`/challenge/pwn --secret okSOD0Cx| /challenge/college`
The Flag is:
>pwn.college{okSOD0CxLMzKS8_xnNVo48YO1oO.dFjM5QDL4YjN0czW}

## Writing to multiple programs
Pipe `/challenge/hack` to `/challenge/the and /challenge/ planet`
`/challenge/hack | tee >(/challenge/the) | /challenge/planet` gives the flag as :


The flag is :
>pwn.college{ke9iG223_Dr-C6CVyQ0FwxjBHXg.dBDO0UDL4YjN0czW}

## Split-piping stderr and stdout


