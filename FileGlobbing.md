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

## Matching with ?
Works like * but only matches single character
`cd /?ha??enge` to change directory to the `challenge` and then running the final command 
The flag is :
>pwn.college{84swACfsEM61cTSrKnNLLK5sFQZ.dJjM4QDL4YjN0czW}

## Matching with []
Instead of matching characters it matches the subset of characters put in []
`/challenge/run file_[bash]` gets the flag 
>pwn.college{kCk3qqYXH7deMltoyHGSt99nOqI.dNjM4QDL4YjN0czW}

## Matching paths with []
Globbing happens on path basis so we can enter paths as arguments as well

The flag is :
>pwn.college{Eo_-iL5Qonz9S54jLRJIkru8OmH.dRjM4QDL4YjN0czW}

## Mixing Globs
cd to `/challenges/files`
for extracting files named as challenge , education , pwning , use[] to wildcard initials and * to wildcard remaining characters.
The flag is :
>pwn.college{4lAmfaNw9FjHVqT-lonH7pdkN7a.dVjM4QDL4YjN0czW}

## Exclusionary Globbing
If the first character in the brackets is a ! or (in newer versions of bash) a ^,
the glob inverts, and that bracket instance matches characters that aren't listed.

change directory to `/challenge/files` using cd 
run `/challenge/run [!pwn]*` to get the flag , this searches for all the files which doesnt start with p, w, n. 

The flag is : 
>pwn.college{I9MBoTgHIAVczGsz5PalagbSH97.dZjM4QDL4YjN0czW}

