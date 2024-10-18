Talks about permissions and how to change them 

For example if ` rw-r--r--` permission is there, it usually decodes to::

r: the user that owns the file (user hacker) can read it
w: the user that owns the file (user hacker) can write to it
-: the user that owns the file (user hacker) cannot execute it
r: users in the group that owns the file (group hacker) can read it
-: users in the group that owns the file (group hacker) cannot write to it
-: users in the group that owns the file (group hacker) cannot execute it
r: all other users can read it
-: all other users cannot write to it
-: all other users cannot execute it

simillary we can use chmod with +r/-r and similar functions . 

In this challenge we change permission to read mode and then cat the flag 
It will look something like : 
![image](https://github.com/user-attachments/assets/f6610ff7-3171-4157-a375-917eaa2a1064)










The flag is : 
>pwn.college{sze8tdk0loCLJLEFamFDCBj29Wo.dNzNyUDL4YjN0czW}
