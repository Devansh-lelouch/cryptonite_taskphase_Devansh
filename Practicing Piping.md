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

The flag is :
>pwn.college{AkWA5fjtbOesHNSFCeWZCj5PDPS.dhTM4QDL4YjN0czW}
