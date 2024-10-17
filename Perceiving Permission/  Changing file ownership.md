Every file in linux is owned by the user on the system. 

root is the administrative account and in most hacking objective is to take over this account 

We change ownership of files using `chown` which stands for change ownership. 
Usually chown can only be invoked by the root user . 

The terminal looks like : 
![image](https://github.com/user-attachments/assets/70683cde-d4fa-4bf6-8456-52039553e2ec)

We are using `chown hacker /flag` to change the owner of /flag to hacker and then reading it 
via cat .

The flag is :
>pwn.college{AWcqMdXXsI2kCnz2kj_ICvzjCvO.dFTM2QDL4YjN0czW}
