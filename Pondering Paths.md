# Module Introduction
In this module we learn about linux file paths.
A root is the directory of the file , it starts with `/`
We refer to files and directories by there paths.

## The Root 
We are invoking `pwn` program by using its absolute path

Type in `/pwn`
The flag is :
>pwn.college{wZdhrZQtZGJRn1m7CZfx3bxfxvZ.dhzN5QDL4YjN0czW}

## Program with absolute paths

We need to invoke a file which is inside another directory which is in turn
inside another directory. 

`/challenge/run` first goes inside `/` directory and then in `challenge`
and finally accesses the file `run`

The flag is :
>pwn.college{QMHsmYRqCCRTvklTMq4SjlIgK0y.dVDN1QDL4YjN0czW}

## Position thy self
`cd` command is used to change directory 
We have to change directory to get into `/usr/share/doc/fontconfig` and then run 
`/challenge/run`

the correct program would look like 
>hacker@paths~position-thy-self:~$ cd /usr/share/doc/fontconfig
hacker@paths~position-thy-self:/usr/share/doc/fontconfig$ /challenge/run

The Flag is :
>pwn.college{wcYC4Solqh-1e0pUK1nz691tw-R.dZDN1QDL4YjN0czW}


## Position Elsewhere
Same as the previous challenge.

## Position Yet Elsewhere
Same as 'Position thy self'

## Implicit Relative Paths
A relative path is any path that does not start at root (i.e., it does not start with /).
A relative path is interpreted relative to your current working directory (cwd).
Your cwd is the directory that your prompt is currently located at.

We cd to `/` directory and then we run the file `challenge/run`

The flag is :
>pwn.college{Qqmgq1-qpw_jDsS9UDdug8oeinP.dlDN1QDL4YjN0czW}

## Explicit relative Paths
Directories have two implicit enteries . and .. 
Using . would refer to the same directory. 

In the challenge we first cd to `/` directory and then use `./` in the start 
to access `challenge/run`

The flag is :
>pwn.college{Qqmgq1-qpw_jDsS9UDdug8oeinP.dlDN1QDL4YjN0czW}

## Implicit Relative Paths
Based on similar concept as previous one we have to use `cd` to go to `/challenge ` path and then invoke 
`./run` file 

The Flag is :
>pwn.college{Ap-QRs7ETeO6w0XdVi6Ey1uMT01.dFTN1QDL4YjN0czW}

## Home Sweet Home
Every user is has a home directory and it is where most of the personal files are stored 

`~` is used as a shorthand for the home directory 
cd will use your home directory as the default destination:

Let the argument where the flag will be copied be `~/k`

The flag is :
> pwn.college{k5kUCYuF3ep9jm48ixN2Txlyw0z.dNzM4QDL4YjN0czW}
