Its some kind of game round of 8 ( stupid game ) 

At the start of the game : 
  Current permissions - 
    User: Read and Write
    Group: Read only
    World : Read only 

 Permission needed:
     User: Read and Write
     Group : No permission
     World : Read only 

So at the first step we have to remove the read permission of the group 

```
chmod g-r /challenge/pwn  #Round1

chmod a=rw /challenge/pwn   #sets read and write permission to all user/group/world  Round2

chmod u=w,g=rw,o=w /challenge/pwn  #Round3

chmod u=w,g=rwx,o=w /challenge/pwn #Round4

chmod u=wx,g=rwx,o=w /challenge/pwn  #Round5

 chmod u=w,g=rwx,o=w /challenge/pwn  #Round6

chmod u=rw,g=rwx,o=rw /challenge/pwm  #Round7

chmod u=rw,g=rwx,o=w /challenge/pwn  #Round8

```

after this we just have to change permission of `flag` file to make it readable and run cat on it to get the flag.

The flag is :
>pwn.college{Yb2F7bFgyJZaTAaGZKPG9xslMzc.dBTM2QDL4YjN0czW}
