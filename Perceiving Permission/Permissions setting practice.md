u=rw sets read and write permissions for the user, and wipes the execute permission
o=x sets only executable permissions for the world, wiping read and write
a=rwx sets read, write, and executable permissions for the user, group, and world! 


Additionally we can set user/group/world permission different by specifying them with something like :
`chmod u=rw,g=r,o=-` which sets different persmission for user,group and world

WHY IS THIS LEVEL SIMILAR TO THE PREVIOUS ONE ???? 
Okay so i did the previous challenge with a shortcut and now how the pwncollege wanted me to but it works so-- 

```
 chmod u=w,g=rwx,o=w /challenge/pwn  #R1
 chmod u=wx,g=rx,o=rw /challenge/pwn #R2
  chmod u=w,g=x,o=rwx /challenge/pwn #R3
chmod u=w,g=wx,o=rwx /challenge/pwn #R4
chmod u=-,g=-,o=w /challenge/pwn #R5
chmod u=-,g=-,o=rwx /challenge/pwn #R6
chmod u=rx,g=x,o=rx /challenge/pwn #R7
chmod u=-,g=rwx,o=wx /challenge/pwn #R8
```

After this we just add readablity to `/flag` using  and read it using :
```
chmod +r /flag

cat /flag
```

The flag is :
>pwn.college{4VKrN9s-mGQQuXuf81OWkTtS1pa.dNTM5QDL4YjN0czW}
