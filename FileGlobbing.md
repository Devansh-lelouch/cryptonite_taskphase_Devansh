# File Globbing 
We learn globbing in this 5th module 

## Matching with *
Glob * lets you match pattern 
When it encounters a * character in any argument, 
the shell will treat it as "wildcard" and try to replace that argument with any files that match the pattern.
When zero files are matched, by default, the shell leaves the glob unchanged
In this challenge we change the directory using `cd /c*` to challenge and then we run the file 
having challenge to get the flag.

The flag is :
 >pwn.college{84s2uG7hk94FJ2mHC-jrhUcwAnY.dFjM4QDL4YjN0czW}
